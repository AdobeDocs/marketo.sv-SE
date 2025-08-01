---
solution: Marketo Engage
product: marketo
title: RUBRIK
description: Lär dig hur du skapar och hanterar riktlinjer för varumärken.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
exl-id: 34bd5fea-0859-4634-9ddd-ae6fd7a1d423
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 0%

---

# Skapa och hantera varumärken {#brands}

>[!AVAILABILITY]
>
>Du måste godkänna [användaravtalet](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} innan du kan använda AI-assistenten i Adobe Marketo Engage. Kontakta Adobe Account Team (din kontoansvarige) om du vill ha mer information.

Varumärkesriktlinjerna är en detaljerad uppsättning regler och standarder som bygger upp ett varumärkes visuella och verbala identitet. De fungerar som referenser för att upprätthålla en enhetlig varumärkesrepresentation på alla marknadsförings- och kommunikationsplattformar.

I [!DNL Marketo Engage] har du nu möjlighet att ange och ordna din varumärkesinformation manuellt eller överföra varumärkesriktlinjer för automatisk informationshämtning.

## Få tillgång till varumärken {#generative-access}

För att få åtkomst till menyn **[!UICONTROL Brands]** i [!DNL Adobe Marketo Engage] måste användarna beviljas behörigheterna **[!UICONTROL Manage brand kit]** eller **[!UICONTROL Enable AI assistant]**. LÄR DIG MER LÄNK

+++  Lär dig hur du tilldelar varumärkesrelaterade behörigheter

Så här tilldelar du behörigheter för varumärken:

1. Gå till fliken **Roller** i produkten **Behörigheter** och välj önskad **roll**.

1. Klicka på **Redigera** om du vill ändra behörigheterna.

1. Lägg till resursen **AI Assistant** och välj sedan **Hantera varumärkespaket** eller **[!UICONTROL Enable Ai assistant]** i listrutan.

   Observera att behörigheten **[!UICONTROL Enable Ai assistant]** endast ger skrivskyddad åtkomst till menyn **[!UICONTROL Brands]**.

   SCREENSHOT

1. Klicka på **Spara** om du vill använda ändringarna.

   Alla användare som redan har tilldelats den här rollen får sina behörigheter automatiskt uppdaterade.

1. Om du vill tilldela den här rollen till nya användare går du till fliken **Användare** på kontrollpanelen **Roller** och klickar på **Lägg till användare**.

1. Ange användarens namn, e-postadress eller välj i listan och klicka sedan på **Spara**.

1. Om användaren inte har skapats tidigare, se [den här dokumentationen](https://experienceleague.adobe.com/sv/docs/experience-platform/access-control/abac/permissions-ui/users).

+++

## Skapa och hantera ert varumärke {#create-brand-kit}

Om du vill skapa och hantera varumärkesriktlinjerna kan du antingen ange detaljerna själv eller överföra dokumentet med varumärkesriktlinjer så att informationen extraheras automatiskt:

1. Klicka på **[!UICONTROL Brands]** på menyn **[!UICONTROL Create brand]**.

   SCREENSHOT

1. Ange en **[!UICONTROL Name]** för ditt varumärke.

1. Dra och släpp eller markera filen för att ladda upp varumärkesriktlinjerna och extrahera automatiskt relevant varumärkesinformation. Klicka på **[!UICONTROL Create brand]**.

   Processen för informationsextrahering börjar nu. Observera att det kan ta flera minuter att slutföra.

   SCREENSHOT

1. Standarderna för att skapa innehåll och visuellt innehåll är nu automatiskt ifyllda. Bläddra bland de olika flikarna för att anpassa informationen efter behov. [Läs mer](#personalize)

1. På den avancerade menyn i varje avsnitt eller kategori kan du lägga till referenser för att extrahera relevant varumärkesinformation automatiskt.

   Använd alternativen **[!UICONTROL Clear section]** eller **[!UICONTROL Clear category]** om du vill ta bort befintligt innehåll.

   SCREENSHOT

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]** och sedan på **[!UICONTROL Publish]** för att göra din varumärkesriktlinje tillgänglig i AI Assistant.

1. Klicka på **[!UICONTROL Edit brand]** om du vill ändra det publicerade varumärket.

   >[!NOTE]
   >
   >Detta skapar en temporär kopia i redigeringsläge och ersätter den publicerade versionen.

   SCREENSHOT

1. Öppna den avancerade menyn på din **[!UICONTROL Brands]**-kontrollpanel genom att klicka på ikonen TOM för att:

   * Visa varumärke
   * Redigera
   * Duplicera
   * Publicera
   * Avpublicera
   * Ta bort

   SCREENSHOT

Riktlinjerna för ditt varumärke finns nu i listrutan **[!UICONTROL Brand]** i AI Assistant-menyn, vilket gör det möjligt att generera innehåll och resurser som är anpassade till dina specifikationer. Läs mer om AI Assistant - LINK

SCREENSHOT

### Ange ett standardmärke {#default-brand}

Du kan ange att ett standardvarumärke ska tillämpas automatiskt när du genererar innehåll och beräknar justeringspoäng när kampanjer skapas.

Om du vill ange ett standardmärke går du till **[!UICONTROL Brands]**-instrumentpanelen. Öppna den avancerade menyn genom att klicka på ikonen och välja **[!UICONTROL Mark as default brand]**.

SCREENSHOT

## Anpassa ert varumärke {#personalize}

### Om varumärket {#about-brand}

Använd fliken **[!UICONTROL About the brand]** för att etablera varumärkets kärnidentitet, som visar dess syfte, personlighet, tagline och andra definitionsattribut.

1. Börja med att fylla i den grundläggande informationen för ditt varumärke i kategorin **[!UICONTROL Key details]**:

   * **[!UICONTROL Brand Kit Name]**: Ange namnet på varumärkespaketet.

   * **[!UICONTROL When to Use]**: Ange scenarier eller kontexter där varumärkespaketet ska användas.

   * **[!UICONTROL Brand Name]**: Ange varumärkets officiella namn.

   * **[!UICONTROL Brand Description]**: Ge en översikt över vad det här varumärket representerar.

   * **[!UICONTROL Default Tagline]**: Lägg till den primära tagline som är associerad med varumärket.

   SCREENSHOT

1. I kategorin **[!UICONTROL Guiding principles]** klargör du varumärkets huvudriktning och filosofi:

   * **[!UICONTROL Mission]**: Ange varumärkets syfte.

   * **[!UICONTROL Vision]**: Beskriv ditt långsiktiga mål eller önskat framtida tillstånd.

   * **[!UICONTROL Market Positioning]**: Förklara hur ert varumärke är positionerat på marknaden.

   SCREENSHOT

1. I kategorin **[!UICONTROL Core brand values]** klickar du på&quot;Lägg till ikon&quot; för att lägga till varumärkets kärnvärden och fylla i informationen:

   * **[!UICONTROL Value]**: Namnge ett kärnvarumärke.

   * **[!UICONTROL Description]**: Förklara vad det här värdet betyder för ditt varumärke.

   * **[!UICONTROL Behaviors]**: Skapa en kontur för de åtgärder eller attityder som återspeglar det här värdet i praktiken.

   * **[!UICONTROL Manifestations]**: Ge exempel på hur det här värdet uttrycks i varumärken.

   SCREENSHOT

1. Klicka vid behov på&quot;Redigera&quot;-ikonen för att uppdatera eller ta bort ett av ert varumärke.

   SCREENSHOT

Du kan nu anpassa ditt varumärke ytterligare eller [publicera ditt varumärke](#create-brand-kit).

### Skrivstil {#writing-style}

Avsnittet **[!UICONTROL Writing style]** beskriver standarderna för att skriva innehåll, med information om hur språk, formatering och struktur ska användas för att bibehålla tydlighet, konsekvens och konsekvens i alla material.

+++ Tillgänglig kategori och exempel

<table>
  <thead>
    <tr>
      <th>Kategori</th>
      <th>Underkategori</th>
      <th>Riktlinjer, exempel</th>
      <th>Exempel på undantag</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Standarder för att skapa innehåll</td>
      <td>Varumärkesmeddelandestandarder</td>
      <td>Lyft fram innovation och budskap som sätter kunden i första rummet.</td>
      <td>Övertyga inte produktfunktionerna.</td>
    </tr>
    <tr>
      <td>Användning med tagline</td>
      <td>Placera tagline under logotypen på alla digitala marknadsföringsresurser.</td>
      <td>Ändra eller översätt inte tagline.</td>
    </tr>
    <tr>
      <td>Core Messaging</td>
      <td>Viktigt om de viktigaste fördelarna - till exempel ökad produktivitet.</td>
      <td>Använd inte orelaterade värdeförslag.</td>
    </tr>
    <tr>
      <td>Namngivningsstandarder</td>
      <td>Använd enkla, beskrivande namn som "ProScheduler".</td>
      <td>Använd inte komplexa termer eller specialtecken.</td>
    </tr>
    <tr>
      <td rowspan="5">Format för varumärkeskommunikation</td>
      <td>Varumärkespersonalitet</td>
      <td>Lätt och lättåtkomligt.</td>
      <td>Var inte besegrad.</td>
    </tr>
    <tr>
      <td>Skrivmekanism</td>
      <td>Håll meningarna korta och slagkraftiga.</td>
      <td>Använd inte för mycket jargon.</td>
    </tr>
    <tr>
      <td>Situationen - ton</td>
      <td>Bibehåll en professionell ton inom kriskommunikation.</td>
      <td>Avvisa inte supportkommunikation.</td>
    </tr>
    <tr>
      <td>Riktlinjer för Word-val</td>
      <td>Använd ord som"innovativ" och"smart".</td>
      <td>Undvik ord som "billig" eller "hack".</td>
    </tr>
    <tr>
      <td>Språkstandarder</td>
      <td>Följ amerikansk engelska konventioner.</td>
      <td>Blanda inte engelska och amerikanska stavningar.</td>
    </tr>
    <tr>
      <td rowspan="3">Regler för regelefterlevnad</td>
      <td>Varumärkesstandarder</td>
      <td>Använd alltid symbolen ™ eller ®.</td>
      <td>Utelämna inte giltiga symboler vid behov.</td>
    </tr>
    <tr>
      <td>Copyrightstandarder</td>
      <td>Inkludera copyrightmeddelanden i marknadsföringsmaterial.</td>
      <td>Använd inte innehåll från tredje part utan tillstånd.</td>
    </tr>
    <tr>
      <td>Friskrivningsstandarder</td>
      <td>Visa ansvarsfriskrivningar på ett läsligt sätt om digitala resurser.</td>
      <td>Dölj inte ansvarsfriskrivningar i områden som inte är synliga.</td>
    </tr>
</table>

+++

</br>

Så här anpassar du din **[!UICONTROL Writing Style]**:

1. Klicka på DEN HÄR IKONEN på fliken **[!UICONTROL Writing Style]** om du vill lägga till en stödlinje, ett undantag eller ett undantag.

1. Ange din riktlinje, undantag eller undantag och klicka på **[!UICONTROL Add]**.

   SCREENSHOT

1. Välj en av stödlinjerna eller uteslutningen som du vill uppdatera eller ta bort.

1. Klicka på&quot;Redigera&quot; för att redigera exemplet eller på&quot;Ta bort&quot;-ikonen för att ta bort det.

   SCREENSHOT

Du kan nu anpassa ditt varumärke ytterligare eller [publicera ditt varumärke](#create-brand-kit).

### Visual content {#visual-content}

Avsnittet **[!UICONTROL Visual Content]** definierar standarderna för bilder och design och anger de specifikationer som behövs för att upprätthålla en enhetlig och enhetlig varumärkeslook.

+++ Tillgängliga kategorier och exempel

<table>
  <thead>
    <tr>
      <th>Kategori</th>
      <th>Riktlinjer, exempel</th>
      <th>Exempel på undantag</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fotografistandarder</td>
      <td>Använd naturligt ljus för bilder utomhus.</td>
      <td>Undvik överredigerade och pixelerade bilder.</td>
    </tr>
    <tr>
      <td>Illustrationsstandarder</td>
      <td>Använd rena, minimalistiska stilar.</td>
      <td>Undvik alltför komplex användning.</td>
    </tr>
    <tr>
      <td>Ikonstandarder</td>
      <td>Använd ett enhetligt rutnätssystem med 24 pixlar.</td>
      <td>Blanda inte ikondimensioner, använd inkonsekventa linjebredder eller avvika från stödrasterreglerna.</td>
    </tr>
    <tr>
      <td>Riktlinjer för användning</td>
      <td>Välj livsstilsbilder som återspeglar verkliga kunder som använder produkten i professionella miljöer.</td>
      <td>Använd inte bilder som står i strid med varumärkestonen eller som inte är i sitt sammanhang.</td>
    </tr>
</table>

+++

</br>

Så här anpassar du din **[!UICONTROL Visual content]**:

1. Klicka på TOM på fliken **[!UICONTROL Visual content]** om du vill lägga till en stödlinje, ett undantag eller ett exempel.

1. Ange din riktlinje, ditt undantag eller exempel och klicka på **[!UICONTROL Add]**.

   SCREENSHOT

1. Om du vill lägga till en bild som visar korrekt användning väljer du **[!UICONTROL Example]** och klickar på **[!UICONTROL Select image]**. Du kan också lägga till en bild som visar felaktig användning som ett exkluderingsexempel.

   SCREENSHOT

1. Välj en av stödlinjerna eller uteslutningen som du vill uppdatera eller ta bort.

1. Välj en stödlinje eller uteslutning för att uppdatera den. Klicka på ikonen &quot;Ta bort&quot; för att ta bort den.

   SCREENSHOT

Du kan nu anpassa ditt varumärke ytterligare eller [publicera ditt varumärke](#create-brand-kit).
