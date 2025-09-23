---
unique-page-id: 2951220
description: Bygg en rapport om personprestanda med Mobile Platform Columns - Marketo Docs - produktdokumentation
title: Bygg en rapport om personprestanda med Mobile Platform-kolumner
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# Bygg en rapport om personprestanda med Mobile Platform-kolumner {#build-a-people-performance-report-with-mobile-platform-columns}

Följ de här stegen för att skapa en People Performance Report (rapport om personprestanda) med mobilplattformskolumner (iOS/Android).

## Skapa smarta mobillistor {#create-mobile-smart-lists}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/ma.png)

1. Välj ett program.

   ![](assets/two-1.png)

1. Välj **[!UICONTROL New]** under **[!UICONTROL New Local Asset]**.

   ![](assets/three-1.png)

1. Klicka på **[!UICONTROL Smart List]**.

   ![](assets/four-1.png)

1. Skriv ett namn och klicka på **[!UICONTROL Create]**.

   ![](assets/five-1.png)

1. Hitta och dra filtret [!UICONTROL Opened Email] till arbetsytan.

   ![](assets/six-1.png)

1. Ange e-post till **[!UICONTROL is any]**.

   ![](assets/seven.png)

1. Klicka på **[!UICONTROL Add Constraint]** och välj **[!UICONTROL Platform]**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Vi använde filtret [!UICONTROL Opened Email] i detta exempel. Du kan också använda filtret [!UICONTROL Clicked Email] på samma sätt som med plattformsbegränsningen.

1. Ange [!UICONTROL Platform] till **[!UICONTROL iOS]**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Minst en person måste ha öppnat ett av dina e-postmeddelanden på en iOS-enhet för att Marketo automatiska förslag ska kunna hitta det. Om det inte visas kan du skriva in det manuellt och spara.

   Skapa nu en andra smart lista för Android-plattformen. När det är klart går du vidare till nästa avsnitt.

## Skapa en rapport om personprestanda {#create-a-people-performance-report}

1. Under Marknadsföringsaktiviteter väljer du det program som innehåller de smarta listorna **[!UICONTROL iOS]** och **[!UICONTROL Android]**.

   ![](assets/ten.png)

1. Välj **[!UICONTROL New]** under **[!UICONTROL New Local Asset]**.

   ![](assets/eleven.png)

1. Klicka på **[!UICONTROL Report]**.

   ![](assets/twelve.png)

1. Ange typ till **[!UICONTROL People Performance]**.

   ![](assets/thirteen.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/fourteen.png)

   Du klarar dig bra! Nu till nästa avsnitt.

## Lägg till smarta mobillistor som kolumner {#add-mobile-smart-lists-as-columns}

1. Klicka på **[!UICONTROL Setup]** i den rapport du just skapade och dra sedan **[!UICONTROL Custom Columns]** till arbetsytan.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Som standard tittar rapporten People Performance på de senaste 7 dagarna. Du kan ändra tidsramen genom att dubbelklicka på den.

1. Sök efter och markera de smarta listor som du skapade tidigare och klicka på **[!UICONTROL Apply]**.

   ![](assets/sixteen.png)

1. Klicka på **[!UICONTROL Report]** om du vill köra rapporten och se dina data.

   ![](assets/seventeen.png)

   Rätt coolt, eller hur? Snyggt gjort!
