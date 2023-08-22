---
unique-page-id: 4720433
description: Konfigurera protokoll för Marketo - Marketo Docs - produktdokumentation
title: Konfigurera protokoll för Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 9d1b18b2aebde00ae715a072580a8f128d07923e
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 3%

---

# Konfigurera protokoll för Marketo {#configure-protocols-for-marketo}

Om du eller din organisation använder restriktiva brandväggs- eller proxyserverinställningar kan du eller din nätverksadministratör behöva tillåtslista vissa domäner och IP-adressintervall för att Adobe Marketo Engage ska fungera som förväntat.

## Varumärkesinriktade kampanjlandningssidor och e-postmeddelanden {#branded-campaign-landing-pages-and-emails}

Er marknadsföringsgrupp använder Marketo för att skapa varumärkesanpassade kampanjlandningssidor och e-postmeddelanden. För att säkerställa att dessa landningssidor och e-postmeddelanden fungerar behöver de lite hjälp från IT-avdelningen. Ange följande protokoll med den information som din marknadsföringsgrupp ska ha skickat till dig via e-post.

Den här artikeln bör delas med IT-avdelningen på det företag som vill implementera dessa protokoll.

Om IT-teamet begränsar webbåtkomsten via ett tillåtelselista ber du dem lägga till följande domäner (inklusive asterisken) för att tillåta alla Marketo resurser och webbsocketar:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Steg 1: Skapa DNS-poster för landningssidor och e-post {#step-create-dns-records-for-landing-pages-and-email}

**Spårningslänk-CNAME**

Marknadsföringsteamet bör ha skickat två förfrågningar till dig om nya CNAME-poster. Den första gäller för landningssidans URL:er, så att landningssidorna visas i URL:er som återspeglar din domän och inte Marketo (den faktiska värden). Den andra gäller spårningslänkarna som ingår i de e-postmeddelanden de skickar från Marketo.

`1` **Lägg till CNAME för landningssidor**

Lägg till landningssidan CNAME som de skickade dig till din DNS-post, så att `[YourLandingPageCNAME]` pekar på den unika kontosträng som tilldelas dina Marketo-landningssidor. Logga in på din domänregistrators webbplats och ange landningssidan CNAME och kontosträng. Vanligtvis omfattar detta tre fält:

* Alias: Ange `[YourLandingPageCNAME]` (tillhandahålls genom marknadsföring)
* Typ: CNAME
* Peka på: Retur `[MunchkinID].mktoweb.com` (tillhandahålls genom marknadsföring)

`2` **Lägg till CNAME för länkar för e-postspårning**

Lägg till e-postmarknadsföringen CNAME som skickades till dig, så att `[YourEmailCNAME]` pekar på [MktoTrackingLink], standardspårningslänken som Marketo har tilldelat i formatet:\
`[YourEmailCNAME].[YourDomain].com` I CNAME `[MktoTrackingLink]`

Exempel:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` måste vara standarddomänen.

`3` **Meddela marknadsföringsteamet**

Meddela marknadsföringsteamet när du har slutfört den här processen.

`4` **Kontakt [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} för att starta processen med att etablera ett SSL-certifikat.**

Den här processen kan ta upp till tre arbetsdagar att slutföra.

## Steg 2: Tillåtslista IP-adresser för Marketo {#step-allowlist-marketo-ips}

När marknadsföringsgruppen använder Marketo för att skicka testmeddelanden (en bra metod innan de skickar ut e-postmeddelanden) blockeras ibland testmeddelandena av skräppostskydd som förlitar sig på avsändarens IP-adresser för att bekräfta att e-postmeddelandet är giltigt. Lägg till Marketo i tillåtelselista för att försäkra dig om att dessa testmeddelanden kommer fram.

Lägg till de här IP-adresserna till ditt företag i tillåtelselista:

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Vissa antispam-system använder fältet för e-postretursökväg i stället för IP-adressen för att tillåta. I sådana fall är det bästa sättet att tillåtslista&#42;.mktomail.com&#39;, eftersom Marketo använder flera postlådeunderdomäner. Andra antispam-system tillåtslista baserat på Från-adressen. I dessa situationer måste du ta med alla avsändande (&#39;Från&#39;) domäner som din marknadsföringsgrupp använder för att kommunicera med personer/leads.

>[!NOTE]
>
>Postini använder en unik teknik och kräver tillåtslista IP-intervall. Se [Tillåtslista med Postini](https://nation.marketo.com/docs/DOC-1066).

## Steg 3: Konfigurera SPF och DKIM {#step-set-up-spf-and-dkim}

Marknadsföringsteamet ska också ha skickat dig DKIM-information som ska läggas till i din DNS-resurspost (visas även nedan). Följ stegen för att konfigurera DKIM och SPF och meddela sedan marknadsföringsteamet att detta har uppdaterats.

1. Om du vill konfigurera SPF lägger du till följande rad i våra DNS-poster:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Om det redan finns en SPF-post i vår DNS-post lägger du bara till följande:\
   include: mktomail.com

   Ersätt CompanyDomain med webbplatsens huvuddomän (t.ex. &quot;`(company.com/)`&quot;) och CorpIP med IP-adressen till företagets e-postserver (t.ex. &quot;255.255.255.255&quot;). Om du ska skicka e-post från flera domäner via Marketo bör din IT-personal lägga till den här raden för varje domän (på en rad).

1. För DKIM skapar du DNS-resursposter för varje domän som vi vill konfigurera. Nedan visas värdposter och TXT-värden för varje domän som vi ska signera för:

   `[DKIMDomain1]`: Värdposten är `[HostRecord1]` och TXT-värdet är `[TXTValue1]`.

   `[DKIMDomain2]`: Värdposten är `[HostRecord2]` och TXT-värdet är `[TXTValue2]`.

   Kopiera HostRecord och TXTValue för varje DKIMDomain som du har konfigurerat efter följande [anvisningar här](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Glöm inte att verifiera varje domän i Admin > E-post > DKIM när din IT-personal har slutfört det här steget.

## Steg 4: Konfigurera MX-poster för din domän {#step-set-up-mx-records-for-your-domain}

Med en MX-post kan du ta emot e-post till domänen som du skickar e-post från för att bearbeta svar och automatiska svar. Om du skickar från din företagsdomän har du förmodligen redan konfigurerat detta. Annars kan du vanligtvis konfigurera den så att den mappas till företagets domäns MX-post.

## Utgående IP-adresser {#outbound-ip-addresses}

En utgående anslutning upprättas av Marketo Engage till en server på Internet åt dig. Vissa partners/leverantörer som du arbetar med, eller din egen IT-organisation, kan använda tillåtelselista för att begränsa åtkomsten till servrar. I så fall måste du förse dem med utgående IP-adressblock från Marketo Engage som kan läggas till i deras tillåtelselista.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} Flödesåtgärden körs som en del av en smart kampanj. En HTTP-begäran görs till en extern webbtjänst. Om webbtjänstutgivaren använder ett tillåtelselista i brandväggen i nätverket där den externa webbtjänsten finns, måste utgivaren lägga till de IP-adressblock som anges nedan i tillåtelselista.

**CRM-synkronisering**

Marketo Engage [Salesforce CRM-synkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} är integreringsmekanismer som gör utgående HTTP-begäranden till API:er som publiceras av CRM-leverantören. Du måste se till att din IT-organisation inte blockerar något av IP-adressblocken nedan så att den inte kommer åt dina CRM-leverantörs-API:er.

**Utgående IP-adressblock för Marketo Engage**

Följande tabeller omfattar alla Marketo Engage-servrar som gör utgående samtal. Använd listorna nedan om du konfigurerar en IP-tillåtelselista, server, brandvägg, åtkomstkontrollista, säkerhetsgrupp eller tredjepartstjänst för att ta emot utgående anslutningar från Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>IP-block (CIDR-notering)</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
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

<table>
 <tbody>
  <tr>
   <th>Enskild IP-adress</th>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
   <tr>
   <td>44.235.171.179</td>
  </tr>
   <tr>
   <td>35.165.244.220</td>
  </tr>
   <tr>
   <td>52.20.211.99</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
   <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
   <tr>
   <td>54.220.138.65</td>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
 </tbody>
</table>

