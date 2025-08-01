---
unique-page-id: 4720433
description: Konfigurera protokoll för Marketo Engage - Marketo Engage Docs - produktdokumentation
title: Konfigurera protokoll för Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 0%

---

# Konfigurera protokoll för Marketo Engage{#configure-protocols-for-marketo-engage}

Om du eller din organisation använder restriktiva brandväggs- eller proxyserverinställningar kan du eller din nätverksadministratör behöva tillåtslista vissa domäner och IP-adressintervall för att Adobe Marketo Engage ska fungera som förväntat.

Om du behöver hjälp med att implementera protokollen nedan kan du dela den här artikeln med din IT-avdelning. Om de begränsar webbåtkomsten med hjälp av ett tillåtelselista måste de lägga till följande domäner (inklusive asterisken) för att tillåta alla Marketo Engage-resurser och webbsocketar:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Steg 1: Skapa DNS-poster för landningssidor och e-post {#step-create-dns-records-for-landing-pages-and-email}

**Länk-CNAME för spårning**

Marknadsföringsteamet bör ha skickat två förfrågningar till dig om nya CNAME-poster. Den första gäller för landningssidans URL:er, så att landningssidorna visas i URL:er som återspeglar din domän och inte Marketo Engage (den faktiska värden). Den andra gäller spårningslänkarna som ingår i de e-postmeddelanden de skickar från Marketo Engage.

`1` **Lägg till CNAME för landningssidor**

Lägg till landningssidan CNAME som de skickade dig till din DNS-post, så att `[YourLandingPageCNAME]` pekar på den unika kontosträng som tilldelas till dina Marketo Engage landningssidor. Logga in på din domänregistrators webbplats och ange landningssidan CNAME och kontosträng. Vanligtvis omfattar detta tre fält:

* Alias: Ange `[YourLandingPageCNAME]` (tillhandahålls av marknadsföring)
* Typ: CNAME
* Peka på: Ange `[MunchkinID].mktoweb.com` (tillhandahålls av marknadsföring)

`2` **Lägg till CNAME för länkar för e-postspårning**

Lägg till e-postmarknadsföringen CNAME skickade dig så att `[YourEmailCNAME]` pekar på [MktoTrackingLink], standardspårningslänken som Marketo Engage tilldelade, i formatet:
`[YourEmailCNAME].[YourDomain].com` I CNAME `[MktoTrackingLink]`

Exempel:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` måste vara standardprofileringsdomän.

`3` **Meddela ditt marknadsföringsteam**

Meddela marknadsföringsteamet när du har slutfört den här processen.

`4` **Kontakta [Adobe Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} för att starta processen med att etablera ett SSL-certifikat.**

Den här processen kan ta upp till tre arbetsdagar att slutföra.

## Steg 2: Tillåtslista IP-adresser för Marketo Engage {#step-allowlist-marketo-ips}

När marknadsföringsgruppen använder Marketo Engage för att skicka testmeddelanden (en bra metod innan de skickar ut e-postmeddelanden) blockeras ibland testmeddelandena av skräppostskydd som förlitar sig på avsändarens IP-adresser för att bekräfta att e-postmeddelandet är giltigt. Lägg till Marketo Engage i tillåtelselista för att försäkra dig om att dessa testmeddelanden kommer fram.

Lägg till de här IP-adresserna till ditt företag i tillåtelselista:

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Vissa antispam-system använder fältet för e-postretursökväg i stället för IP-adressen för att tillåta. I dessa fall är det bästa sättet att tillåtslista &#42;.mktomail.com eftersom Marketo Engage använder flera postlådeunderdomäner. Andra antispam-system tillåtslista baserat på Från-adressen. I dessa situationer måste du ta med alla avsändande (&#39;Från&#39;) domäner som din marknadsföringsgrupp använder för att kommunicera med personer/leads.

>[!NOTE]
>
>Postini använder en unik teknik och kräver tillåtslista IP-intervall. Se [Tillåtslista med Postini](https://nation.marketo.com/docs/DOC-1066).

## Steg 3: Konfigurera SPF och DKIM {#step-set-up-spf-and-dkim}

Marknadsföringsteamet ska också ha skickat information om DKIM (Domain Keys Identified Mail) till dig för att läggas till i din DNS-resurspost (visas även nedan). Följ stegen för att konfigurera DKIM och SPF (Sender Policy Framework) och meddela sedan marknadsföringsteamet att detta har uppdaterats.

1. Om du vill konfigurera SPF lägger du till följande rad i våra DNS-poster:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   Om det redan finns en SPF-post i vår DNS-post lägger du bara till följande:
include: mktomail.com

   Ersätt CompanyDomain med huvuddomänen för din webbplats (t.ex. `(company.com/)`) och CorpIP med IP-adressen för företagets e-postserver (t.ex. &quot;255.255.255.255&quot;). Om du ska skicka e-post från flera domäner via Marketo Engage bör din IT-personal lägga till den här raden för varje domän (på en rad).

1. För DKIM skapar du DNS-resursposter för varje domän som vi vill konfigurera. Nedan visas värdposter och TXT-värden för varje domän som vi ska signera för:

   `[DKIMDomain1]`: Värdposten är `[HostRecord1]` och TXT-värdet är `[TXTValue1]`.

   `[DKIMDomain2]`: Värdposten är `[HostRecord2]` och TXT-värdet är `[TXTValue2]`.

   Kopiera HostRecord och TXTValue för varje DKIMDomain som du har konfigurerat efter att ha följt [instruktionerna här](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Glöm inte att verifiera alla domäner i Admin > E-post > DKIM när IT-personalen har slutfört det här steget.

## Steg 4: Konfigurera DMARC {#set-up-dmarc}

DMARC (domänbaserad meddelandeautentisering, rapportering och överensstämmelse) är ett autentiseringsprotokoll som används för att hjälpa organisationer att skydda sin domän mot obehörig användning. DMARC utökar befintliga autentiseringsprotokoll, som SPF och DKIM, för att informera mottagarservrar om vilka åtgärder de bör vidta om ett autentiseringsfel inträffar på deras domän. Även om DMARC för närvarande är valfritt rekommenderar vi starkt att det skyddar er organisations varumärke och anseende bättre. Större leverantörer som Google och Yahoo kommer att kräva att DMARC används för bulkavsändare från och med februari 2024.

För att DMARC ska fungera måste du ha minst en av följande DNS TXT-poster:

* En giltig SPF
* En giltig DKIM-post för din FROM: Domän (rekommenderas för Marketo Engage)

Dessutom måste du ha en DMARC-specifik DNS TXT-post för din FROM: Domain. Du kan också ange en e-postadress som du vill använda för att ange var DMARC-rapporter ska ligga inom organisationen, så att du kan övervaka rapporter.

Vi rekommenderar att man långsamt implementerar DMARC genom att eskalera DMARC-policyn från p=none till p=karantän, till p=reject när man får kunskap om DMARC potentiella konsekvenser och ställer in din DMARC-policy på att avlasta anpassningen av SPF och DKIM.

### DMARC Example Workflow {#dmarc-example-workflow}

1. Om du är konfigurerad att ta emot rapporter från DMARC bör du göra följande..

   I. Analysera den feedback och de rapporter som du tar emot och använder (p=none), som instruerar mottagaren att inte vidta några åtgärder mot meddelanden som inte kan autentiseras, men ändå skicka e-postrapporter till avsändaren.

   II. Granska och åtgärda problem med SPF/DKIM om legitimt meddelande inte kan autentiseras.

   III. Kontrollera om SPF eller DKIM är anpassade och skickar autentisering för alla giltiga e-postmeddelanden.

   IV. Granska rapporter för att säkerställa att resultatet blir det du förväntar dig baserat på din SPF/DKIM-policy.

1. Fortsätt att justera principen till (p=karantän), vilket innebär att den mottagande e-postservern ska karantänera e-post som inte kan autentiseras (detta innebär vanligtvis att meddelandena placeras i skräppostmappen).

   I. Granska rapporter för att säkerställa att resultatet blir vad du förväntar dig.

1. Om du är nöjd med beteendet hos meddelanden på p=karantännivå kan du justera principen till (p=avvisad). p=avvisningsprincipen innebär att mottagaren helt nekar (studsar) alla e-postmeddelanden för domänen som inte kan autentiseras. När den här principen är aktiverad har bara e-post som är verifierad som 100 % autentiserad av din domän en chans att placeras i inkorgen.

>[!CAUTION]
>
>Använd den här profilen med försiktighet och kontrollera om den passar din organisation.

### DMARC Reporting {#dmarc-reporting}

DMARC erbjuder möjlighet att få rapporter om e-postmeddelanden som inte godkänns i SPF/DKIM. Det finns två olika rapporter som genereras av ISP-tjänstleverantörer som en del av autentiseringsprocessen som avsändare kan ta emot via RUA/RUF-taggarna i sin DMARC-policy.

* Aggregate Reports (RUA): does not contain any PII (Personally Identiitable Information) that will be GDPR (General Data Protection Regulation) sensitive.

* Forensic Reports (RUF): Innehåller e-postadresser som är GDPR-känsliga. Innan ni börjar använda programmet bör ni kontrollera internt hur ni hanterar information som måste vara GDPR-kompatibel.

Det viktigaste användningsområdet för dessa rapporter är att få en översikt över e-postmeddelanden som försöker förfalskas. Det här är mycket tekniska rapporter som är bäst sammanställda via ett verktyg från tredje part.

### Exempel på DMARC Records {#example-dmarc-records}

* Minsta bandpost: `v=DMARC1; p=none`

* Post som dirigerar till en e-postadress för att ta emot rapporter: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC-taggar och vad de gör {#dmarc-tags-and-what-they-do}

DMARC-poster har flera komponenter som kallas DMARC-taggar. Varje tagg har ett värde som anger en viss aspekt av DMARC.

<table>
<thead>
  <tr>
    <th>Märkordsnamn </th>
    <th>Obligatoriskt/valfritt </th>
    <th>Funktion </th>
    <th>Exempel </th>
    <th>Standardvärde </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>Obligatoriskt</td>
    <td>Den här DMARC-taggen anger versionen. Det finns bara en version från och med nu, så det här har ett fast värde på v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Obligatoriskt</td>
    <td>Visar den valda DMARC-principen och instruerar mottagaren att rapportera, sätta i karantän eller avvisa e-post som inte kan autentiseras.</td>
    <td>p=ingen, karantän eller avvisad</td>
    <td>–</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Valfritt</td>
    <td>Låter domänägaren ange rapportalternativ.</td>
    <td>0: Generera en rapport om allt misslyckas
    <br>1: Generera en rapport om något misslyckas
    <br>d: Generera en rapport om DKIM misslyckas
    <br>s: Generera en rapport om SPF misslyckas</td>
    <td>1 (rekommenderas för DMARC-rapporter)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Valfritt</td>
    <td>Anger procentandelen meddelanden som ska filtreras.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Valfritt (rekommenderas)</td>
    <td>Identifierar var aggregerade rapporter kommer att levereras.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>–</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Valfritt (rekommenderas)</td>
    <td>Identifierar var kriminaltekniska rapporter kommer att levereras.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>–</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Valfritt</td>
    <td>Anger DMARC-princip för underdomäner till den överordnade domänen.</td>
    <td>sp=avvisa</td>
    <td>–</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Valfritt</td>
    <td>Kan antingen vara Strikt (Strikt) eller Avspänd ®. Avspänd justering innebär att den domän som används i DKIM-signaturen kan vara en underdomän till Från-adressen. Strikta justeringar innebär att den domän som används i DKIM-signaturen måste vara en exakt matchning av den domän som används i Från-adressen.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Valfritt</td>
    <td>Kan antingen vara Strikt (Strikt) eller Avspänd ®. Avspänd justering innebär att ReturnPath-domänen kan vara en underdomän till Från adress. Strikta justeringar innebär att domänen Return-Path måste vara exakt densamma som Från-adressen.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Mer information om DMARC och alla dess alternativ finns på [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC och Marketo Engage {#dmarc-and-marketo-engage}

Det finns två typer av justering för DMARC - DKIM-justering och SPF-justering.

>[!NOTE]
>
>Vi rekommenderar att du justerar DMARC på DKIM mot SPF för Marketo Engage.

* DKIM-justerad DMARC - För att kunna konfigurera DKIM-anpassade DMARC måste du:

   * Konfigurera DKIM för Från: Meddelandets domän. Använd instruktionerna [ i den här artikeln](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Konfigurera DMARC för FROM:/DKIM-domänen som konfigurerats tidigare

* DMARC-justerad SPF - Om du vill konfigurera DMARC-justerad SPF via varumärkesanpassad retursökväg måste du:

   * Konfigurera domänen för varumärkesskyddad retursökväg
      * Konfigurera lämplig SPF-post
      * Ändra MX-posten så att den pekar tillbaka till standardvärdet för MX för det datacenter som e-postmeddelandet skickas från

   * Konfigurera DMARC för domänen för varumärkesskyddad retursökväg

* Om du skickar e-post från Marketo Engage via en dedikerad IP-adress och inte redan har implementerat en profilerad retursökväg, eller om du inte är säker på om du har det, öppnar du en biljett med [Adobe Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Om du skickar e-post från Marketo Engage via en delad pool med IP-adresser kan du se om du är berättigad till betrodda IP-adresser genom att [tillämpa här](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. Varumärkesbaserad retursökväg erbjuds kostnadsfritt till dem som skickar från Marketo Engage Betrodda IP-adresser. Om du godkänner programmet kan du kontakta Adobe Support för att skapa en egen returväg.

   * Betrodda IP-adresser: En delad pool med IP-adresser som är reserverade för användare med lägre volym som skickar &lt;75 kB/månad och som inte är kvalificerade för en dedikerad IP-adress. Dessa användare måste också uppfylla kraven på god praxis.

* Om du skickar e-post från Marketo Engage via delade IP-adresser och du inte är berättigad till betrodda IP-adresser och skickar mer än 100 000 meddelanden per månad måste du kontakta Adobe Account Team (din kontohanterare) för att köpa en dedikerad IP-adress.

* Strikta SPF-justeringar stöds inte och rekommenderas inte i Marketo Engage.

## Steg 5: Konfigurera MX-poster för din domän {#step-set-up-mx-records-for-your-domain}

Med en MX-post kan du ta emot e-post till domänen som du skickar e-post från för att bearbeta svar och automatiska svar. Om du skickar från din företagsdomän har du förmodligen redan konfigurerat detta. Annars kan du vanligtvis konfigurera den så att den mappas till företagets domäns MX-post.

## Utgående IP-adresser {#outbound-ip-addresses}

En utgående anslutning upprättas av Marketo Engage till en server på Internet åt dig. Vissa partners/leverantörer som du arbetar med, eller din egen IT-organisation, kan använda tillåtelselista för att begränsa åtkomsten till servrar. Om så är fallet måste du förse dem med utgående IP-adressblock från Marketo Engage som kan läggas till i deras tillåtelselista.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} är en utgående integreringsmekanism. När en [anropswebbkrok](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"}-flödesåtgärd körs som en del av en smart kampanj, görs en HTTP-begäran till en extern webbtjänst. Om webbtjänstutgivaren använder ett tillåtelselista i brandväggen i nätverket där den externa webbtjänsten finns, måste utgivaren lägga till de IP-adressblock som anges nedan i tillåtelselista.

**CRM-synkronisering**

Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} och [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} är integreringsmekanismer som gör utgående HTTP-begäranden till API:er som publiceras av CRM-leverantören. Du måste se till att din IT-organisation inte blockerar något av IP-adressblocken nedan så att den inte kommer åt dina CRM-leverantörs-API:er.

**Utgående IP-adressblock för Marketo Engage**

Följande tabeller omfattar alla Marketo Engage-servrar som gör utgående samtal. Använd listorna nedan om du konfigurerar en IP-tillåtelselista, server, brandvägg, åtkomstkontrollista, säkerhetsgrupp eller tredjepartstjänst för att ta emot utgående anslutningar från Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>IP-block (CIDR-notering)</th>
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
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.5.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
