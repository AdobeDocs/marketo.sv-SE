---
unique-page-id: 4720433
description: Konfigurera protokoll för Marketo - Marketo Docs - produktdokumentation
title: Konfigurera protokoll för Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 56f429dabf19c4425c68b0dcd745621681a038ae
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 1%

---

# Konfigurera protokoll för Marketo {#configure-protocols-for-marketo}

Om du eller din organisation använder restriktiva brandväggs- eller proxyserverinställningar kan du eller din nätverksadministratör behöva tillåtslista vissa domäner och IP-adressintervall för att Adobe Marketo Engage ska fungera som förväntat.

## Varumärkesinriktade kampanjlandningssidor och e-postmeddelanden {#branded-campaign-landing-pages-and-emails}

Er marknadsföringsgrupp använder Marketo för att skapa varumärkesanpassade kampanjlandningssidor och e-postmeddelanden. För att säkerställa att dessa landningssidor och e-postmeddelanden fungerar behöver de lite hjälp från IT-avdelningen. Ange följande protokoll med den information som din marknadsföringsgrupp ska ha skickat till dig via e-post.

Den här artikeln bör delas med IT-avdelningen på det företag som vill implementera dessa protokoll.

>[!NOTE]
>
>Om IT-teamet begränsar webbåtkomsten via ett tillåtelselista ber du dem lägga till följande domäner (inklusive asterisken) för att tillåta alla Marketo resurser och webbsocketar:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`

## Steg 1: Skapa DNS-poster för landningssidor och e-post {#step-create-dns-records-for-landing-pages-and-email}

**Spårningslänk-CNAME**

Marknadsföringsteamet bör ha skickat två förfrågningar till dig om nya CNAME-poster. Den första gäller för landningssidans URL:er, så att landningssidorna visas i URL:er som återspeglar din domän och inte Marketo (den faktiska värden). Den andra gäller spårningslänkarna som ingår i de e-postmeddelanden de skickar från Marketo.

`1` **Lägg till CNAME för landningssidor**

Lägg till landningssidan CNAME som de skickade dig till din DNS-post, så att `[YourLandingPageCNAME]` pekar på den unika kontosträng som tilldelas dina Marketo-landningssidor. Logga in på din domänregistrators webbplats och ange landningssidan CNAME och kontosträng. Vanligtvis omfattar detta tre fält:

* Alias: Retur `[YourLandingPageCNAME]` (tillhandahålls genom marknadsföring)
* Typ: CNAME
* Peka på: Retur `[MarketoAccountString].mktoweb.com` (tillhandahålls genom marknadsföring)

`2` **Lägg till CNAME för länkar för e-postspårning**

Lägg till e-postmarknadsföringen CNAME som skickades till dig, så att `[YourEmailCNAME]` pekar på [MktoTrackingLink], standardspårningslänken som Marketo har tilldelat i formatet:\
`[YourEmailCNAME].[YourDomain].com` I CNAME `[MktoTrackingLink]`

Till exempel:

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Meddela marknadsföringsteamet**

Meddela marknadsföringsteamet när du har slutfört den här processen.

`4` **Kontakt [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} för att starta etableringen av ett SSL-certifikat.**

Den här processen kan ta upp till tre arbetsdagar att slutföra.

## Steg 2: IP-adresser för Tillåtelselista Marketo {#step-allowlist-marketo-ips}

När marknadsföringsgruppen använder Marketo för att skicka testmeddelanden (en bra metod innan de skickar ut e-postmeddelanden) blockeras ibland testmeddelandena av skräppostskydd som förlitar sig på avsändarens IP-adresser för att bekräfta att e-postmeddelandet är giltigt. Lägg till Marketo i tillåtelselista för att försäkra dig om att dessa testmeddelanden kommer fram.

Lägg till de här IP-adresserna till ditt företag i tillåtelselista:

199.15.212.0/22\
192.28.144.0/20 192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Vissa antispam-system använder fältet för e-postretursökväg i stället för IP-adressen för att tillåta. I sådana fall är det bästa sättet att gå till tillåtelselista&quot;&#42;.mktomail.com&quot;, eftersom Marketo använder flera postlådeunderdomäner. Andra antispam-system tillåtslista baserat på Från-adressen. I dessa situationer måste du se till att inkludera alla avsändande (&quot;Från&quot;) domäner som din marknadsföringsgrupp använder för att kommunicera med personer/leads.

>[!NOTE]
>
>Postini använder en unik teknik och kräver tillåtslista IP-intervall. Se [Tillåtslista med Postini](https://nation.marketo.com/docs/DOC-1066).

## Steg 3: Konfigurera SPF och DKIM {#step-set-up-spf-and-dkim}

Marknadsföringsteamet ska också ha skickat dig DKIM-information som ska läggas till i din DNS-resurspost (visas även nedan). Följ stegen för att konfigurera DKIM och SPF och meddela sedan marknadsföringsteamet att detta har uppdaterats.

1. Om du vill konfigurera SPF lägger du till följande rad i våra DNS-poster:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   inkludera: mktomail.com ~alla

   Om det redan finns en SPF-post i vår DNS-post lägger du bara till följande:\
   inkludera: mktomail.com

   Ersätt CompanyDomain med webbplatsens huvuddomän (t.ex.: &quot;`(company.com/)`&quot;) och CorpIP med IP-adressen till företagets e-postserver (t.ex. &quot;255.255.255.255&quot;). Om du ska skicka e-post från flera domäner via Marketo bör din IT-personal lägga till den här raden för varje domän (på en rad).

1. För DKIM skapar du DNS-resursposter för varje domän som vi vill konfigurera. Nedan visas värdposter och TXT-värden för varje domän som vi ska signera för:

   `[DKIMDomain1]`: Värdposten är `[HostRecord1]` och TXT-värdet är `[TXTValue1]`.

   `[DKIMDomain2]`: Värdposten är `[HostRecord2]` och TXT-värdet är `[TXTValue2]`.

   Kopiera HostRecord och TXTValue för varje DKIMDomain som du har konfigurerat efter följande [anvisningar](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Glöm inte att verifiera varje domän i Admin > E-post > DKIM när din IT-personal har slutfört det här steget.

## Steg 4: Konfigurera MX-poster för din domän {#step-set-up-mx-records-for-your-domain}

Med en MX-post kan du ta emot e-post till domänen som du skickar e-post från för att bearbeta svar och automatiska svar. Om du skickar från din företagsdomän har du förmodligen redan detta konfigurerat. Annars kan du vanligtvis konfigurera den så att den mappas till företagets domäns MX-post.

## Utgående IP-adresser {#outbound-ip-addresses}

En utgående anslutning upprättas av Marketo Engage till en server på Internet åt dig. Vissa partners/leverantörer som du arbetar med, eller din egen IT-organisation, kan använda tillåtelselista för att begränsa åtkomsten till servrar. I så fall måste du förse dem med utgående IP-adressblock från Marketo Engage som kan läggas till i deras tillåtelselista.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;} är en utgående integreringsmekanism. När en [Ring webkrok](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md)Flödesåtgärden {target=&quot;_blank&quot;} körs som en del av en smart kampanj, en HTTP-begäran görs till en extern webbtjänst. Om webbtjänstutgivaren använder ett tillåtelselista i brandväggen i nätverket där den externa webbtjänsten finns, måste utgivaren lägga till de IP-adressblock som anges nedan i tillåtelselista.

**CRM-synkronisering**

Marketo Engage [Salesforce CRM-synkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;} och [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;} är integreringsmekanismer som gör utgående HTTP-begäranden till API:er som publiceras av CRM-leverantören. Du måste se till att din IT-organisation inte blockerar något av IP-adressblocken nedan så att den inte kommer åt dina CRM-leverantörs-API:er.

**Utgående IP-adressblock för Marketo Engage**

Följande tabell omfattar alla Marketo Engage-servrar som gör utgående samtal. Använd den här listan om du konfigurerar en IP-tillåtelselista, server, brandvägg, åtkomstkontrollista, säkerhetsgrupp eller tredjepartstjänst för att ta emot utgående anslutningar från Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>IP-block (CIDR-notering)</th>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
   <tr>
   <td>192.28.160.0/19</td>
  </tr>
   <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>
