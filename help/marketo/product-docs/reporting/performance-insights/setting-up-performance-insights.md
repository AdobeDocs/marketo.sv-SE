---
unique-page-id: 12981145
description: Ställa in prestandainsikter - Marketo Docs - produktdokumentation
title: Konfigurera prestandainsikter
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 2%

---

# Konfigurerar [!UICONTROL Performance Insights] {#setting-up-performance-insights}

Följ stegen nedan för att konfigurera MPI.

## Inställningar för affärsmöjlighet {#opportunity-setup}

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicka på **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Om du inte har någon RCA måste du välja **[!UICONTROL Program Analysis]** för steg 2.

1. Klicka på **[!UICONTROL Edit]** under Attribution.

   ![](assets/three-1.png)

1. Attributinställningar visas.

   ![](assets/four-2.png)

   Om attribuering är explicit kontrollerar du att säljprojektskontaktrollen har fyllts i (antingen via slutpunkten för säljprojektsrollen eller via CRM-integrering).

   Om Attribution är implicit kontrollerar du att företagsfältet på leadet/kontakten är samma som kontonamnet för affärsmöjligheten.

   >[!NOTE]
   >
   >Se till att rätt fält fylls i för alla affärsmöjligheter:
   >
   >* [!UICONTROL Opportunity Amount]
   >* [!UICONTROL Is Closed]
   >* [!UICONTROL Is Won]
   >* [!UICONTROL Creation Date] (detta kanske inte är inställt i ditt fall)
   >* [!UICONTROL Closed Date] (detta kanske inte är inställt i ditt fall)
   >* [!UICONTROL Opportunity Type]

## Programinställningar {#program-setup}

Uppdatera programkostnaderna i minst 12 månader. Du kan göra detta manuellt eller med program-API:t. I det här exemplet gör vi det manuellt.

1. Klicka på **[!UICONTROL Marketing Activities]**.

   ![](assets/ma.png)

1. Hitta och välj program.

   ![](assets/select-program.png)

1. Klicka på fliken **[!UICONTROL Setup]**.

   ![](assets/setup-tab.png)

1. Dra **[!UICONTROL Period Cost]** till arbetsytan.

   ![](assets/period-cost.png)

1. Ange programmånaden för minst 12 månader sedan och klicka på **[!UICONTROL Ok]**.

   ![](assets/set-period.png)

1. Ange periodkostnaden och klicka på **[!UICONTROL Save]**.

   ![](assets/set-cost.png)

Granska sedan analysbeteendet för att ange om en viss kanal ska inkluderas i analysen. Ange analysbeteende (normal, inkluderande, operativ).

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicka på **[!UICONTROL Tags]**.

   ![](assets/tags.png)

1. Klicka på **+** för att utöka kanallistan.

   ![](assets/channel.png)

1. Dubbelklicka på den önskade kanalen.

   ![](assets/channel-click.png)

1. Klicka på listrutan **[!UICONTROL Analytics Behavior]** och välj önskat beteende.

   ![](assets/edit-channel.png)

1. Ange kriterier för framgång.

   ![](assets/success.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/save.png)

## Koppla programmet till personen {#tie-the-program-to-the-person}

1. Kontrollera att inköpsprogrammet och förvärvsdatumet har angetts för varje person i databasen för att First Touch Attribution ska fungera.
1. Se till att era program är framgångslägen för era medarbetare.

>[!NOTE]
>
>Ändringarna görs inte omedelbart. En nattetid krävs innan ändringarna träder i kraft.
