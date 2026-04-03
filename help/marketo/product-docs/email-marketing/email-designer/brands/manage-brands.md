---
solution: Marketo Engage
product: Marketo
title: Hantera varumärke
description: Läs om hur du skapar och hanterar varumärkesriktlinjer i e-postmeddelandet om Designer. Konfigurera och uppdatera varumärkesinställningar för dina e-postmeddelanden.
role: User
level: Beginner, Intermediate
badge: Beta
exl-id: 88945b7c-0205-4540-bb37-1df85e647d90
source-git-commit: 1850dd03baba259e99e8cc089b39f35735e63fdf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Skapa och hantera varumärken {#create-and-manage-brands}

Varumärkesriktlinjerna är en detaljerad uppsättning regler och standarder som bygger upp ett varumärkes visuella och verbala identitet. De fungerar som referenser för att upprätthålla en enhetlig varumärkesrepresentation på alla marknadsförings- och kommunikationsplattformar.

Ange och ordna varumärkesinformation manuellt eller överför riktlinjer för varumärken för automatisk informationshämtning.

>[!AVAILABILITY]
>
>Du måste godkänna [användaravtalet](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} innan du kan använda AI-assistenten i Adobe Marketo Engage. Kontakta din kontoansvarige på Adobe om du vill ha mer information.

## Få tillgång till varumärken {#access}

För att få åtkomst till menyn **[!UICONTROL brands]** i [!DNL Adobe Marketo Engage] måste användarna få behörighet.

+++  Lär dig hur du tilldelar varumärkesrelaterade behörigheter

### Användare och roller {#users-and-roles}

1. I _Admin_ väljer du **Användare och roller**.

1. Välj önskad roll.

1. Klicka för att expandera menyn **Access Design Studio**.

1. Välj **Access AI Assistant** och klicka på **Spara**.

+++

## Skapa och hantera ert varumärke {#create-brand-kit}

Om du vill skapa och hantera varumärkesriktlinjerna kan du antingen ange detaljerna själv eller överföra dokumentet med varumärkesriktlinjer så att informationen extraheras automatiskt.

1. I _Admin_ väljer du **Ny upplevelse**.

   ![](assets/create-and-manage-brands-5.png)

1. Klicka på _Redigera_ bredvid **Hantera dina varumärken**.

   ![](assets/create-and-manage-brands-6.png)

1. Klicka på **[!UICONTROL Create brand]**.

1. Ange en **[!UICONTROL Name]** för ditt varumärke.

1. Dra och släpp eller välj din PDF för att ladda upp varumärkesriktlinjerna och extrahera automatiskt relevant varumärkesinformation. Klicka på **[!UICONTROL Create]**.

   Informationsextraheringsprocessen börjar. Det kan ta flera minuter.

   ![](assets/create-and-manage-brands-7.png)

1. Standarderna för innehåll och visuellt skapande fylls nu i automatiskt. Bläddra bland de olika flikarna för att anpassa informationen efter behov.

1. På den avancerade menyn i varje avsnitt eller kategori kan du lägga till referenser för att extrahera relevant varumärkesinformation automatiskt.

   Använd alternativen **[!UICONTROL Clear section]** eller **[!UICONTROL Clear category]** om du vill ta bort befintligt innehåll.

   ![](assets/create-and-manage-brands-8.png){width="800" zoomable="yes"}

   ![](assets/create-and-manage-brands-9.png){width="800" zoomable="yes"}

1. Klicka på **Filter** om du vill filtrera riktlinjer efter kanal- eller elementtyp.

   ![](assets/create-and-manage-brands-10.png)

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]** och sedan på **[!UICONTROL Publish]** för att göra din varumärkesriktlinje tillgänglig i AI Assistant.

1. Klicka på **[!UICONTROL Edit brand]** om du vill ändra det publicerade varumärket.

   >[!NOTE]
   >
   >Detta skapar en temporär kopia i redigeringsläge och ersätter den aktiva versionen när den har publicerats.

   ![](assets/create-and-manage-brands-11.png)

1. Öppna den avancerade menyn på din **[!UICONTROL Brands]**-kontrollpanel genom att klicka på ikonen med tre punkter för att:

* Visa varumärke
* Redigera
* Duplicera
* Publicera
* Avpublicera
* Ta bort

  ![](assets/create-and-manage-brands-12.png)

Riktlinjerna för ditt varumärke finns nu i listrutan **[!UICONTROL Brand]** i AI Assistant-menyn, vilket gör det möjligt att generera innehåll och resurser som är anpassade till dina specifikationer.

### Ange ett standardmärke {#default-brand}

Du kan ange att ett publicerat varumärke ska användas som standard när du genererar innehåll och beräknar justeringspoäng när kampanjer skapas.

Om du vill ange ett standardmärke går du till **[!UICONTROL Brands]**-instrumentpanelen. Öppna den avancerade menyn genom att klicka på ikonen med tre punkter och välja **[!UICONTROL Mark as default brand]**.

![](assets/create-and-manage-brands-13.png)
