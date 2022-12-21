---
unique-page-id: 2951220
description: Bygg en rapport om personprestanda med Mobile Platform Columns - Marketo Docs - produktdokumentation
title: Bygg en rapport om personprestanda med Mobile Platform-kolumner
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Bygg en rapport om personprestanda med Mobile Platform-kolumner {#build-a-people-performance-report-with-mobile-platform-columns}

Följ de här stegen för att skapa en rapport om personprestanda med mobilplattformskolumner (iOS/Android).

## Skapa smarta mobillistor {#create-mobile-smart-lists}

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Välj ett program.

   ![](assets/two-1.png)

1. Under **Nytt**, markera **Ny lokal resurs**.

   ![](assets/three-1.png)

1. Klicka **Smart List**.

   ![](assets/four-1.png)

1. Skriv ett namn och klicka på **Skapa**.

   ![](assets/five-1.png)

1. Hitta och dra filtret Öppen e-post till arbetsytan.

   ![](assets/six-1.png)

1. Ange e-post till **är**.

   ![](assets/seven.png)

1. Klicka på **Lägg till begränsning** och markera **Plattform**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Vi använde filtret Öppen e-post i det här exemplet. Du kan också använda det klickade e-postfiltret på samma sätt som det har plattformsbegränsningen.

1. Ange plattform till **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Minst en person måste ha öppnat ett av dina e-postmeddelanden på en iOS-enhet för att Marketo automatiska förslag ska kunna hitta det. Om det inte visas kan du skriva in det manuellt och spara.

   Skapa nu en andra smart lista för Android-plattformen. När det är klart går du vidare till nästa avsnitt.

## Skapa en rapport om personprestanda {#create-a-people-performance-report}

1. Under Marknadsföringsaktiviteter väljer du det program som du har **iOS** och **Android** smarta listor.

   ![](assets/ten.png)

1. Under **Nytt**, markera **Ny lokal resurs**.

   ![](assets/eleven.png)

1. Klicka **Rapport**.

   ![](assets/twelve.png)

1. Ange typ till **Personprestanda**.

   ![](assets/thirteen.png)

1. Klicka **Skapa**.

   ![](assets/fourteen.png)

   Du klarar dig bra! Nu till nästa avsnitt.

## Lägg till smarta mobillistor som kolumner {#add-mobile-smart-lists-as-columns}

1. Klicka på **Inställningar** och sedan dra **Egna kolumner** på arbetsytan.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Som standard tittar rapporten People Performance på de senaste 7 dagarna. Du kan ändra tidsramen genom att dubbelklicka på den.

1. Sök efter och markera de smarta listor du skapade tidigare och klicka på **Använd**.

   ![](assets/sixteen.png)

1. Klicka **Rapport** för att köra rapporten och se dina data.

   ![](assets/seventeen.png)

   Rätt coolt, eller hur? Snyggt gjort!
