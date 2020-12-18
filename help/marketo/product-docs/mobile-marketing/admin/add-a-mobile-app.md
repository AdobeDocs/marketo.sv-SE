---
unique-page-id: 7512252
description: Lägg till en mobilapp - Marketo Docs - Produktdokumentation
title: Lägg till en mobilapp
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Lägg till en mobilapp {#add-a-mobile-app}

Skicka push-meddelanden till kundbasen genom att ansluta mobilappen till Marketo.

Program startar normalt i en sandlådemiljö, där inledande utveckling och testning utförs. Utvecklarna använder sedan en produktionsmiljö för att bygga den slutliga app som ska användas av kunderna. Du måste välja lämpligt meddelandecertifikat när du lägger till en mobilapp (se steg 4 nedan).

>[!NOTE]
>
>**Tillgänglighet**
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Klicka på **Admin**.

   ![](assets/image2015-4-22-16-3a12-3a32.png)

1. Klicka** Mobilappar och enheter**.

   ![](assets/image2016-1-12-15-3a42-3a30.png)

   Klicka på Ny mobilapp.

   ![](assets/image2015-4-22-16-3a17-3a15.png)

1. Ange ett namn. I listrutan **Typ** väljer du den typ av miljö som du använder - Sandbox eller Production. Klicka på **Spara**.

   ![](assets/image2015-11-18-15-3a52-3a15.png)

   >[!NOTE]
   >
   >Vi rekommenderar att du använder ett produktionsmeddelandecertifikat i en produktionsmiljö. Ett sandlådecertifikat installeras i en produktionsmiljö utan problem, men du får inga meddelanden. Om du har några frågor om din miljö eller ditt meddelandecertifikat kontaktar du Marketo Admin eller Mobile Apps Developer.

   Snyggt! Nu ska vi konfigurera appen så att den fungerar med Android- och iOS-enheter.

>[!MORELIKETHIS]
>
>* [Konfigurera Android-åtkomst för mobilapp](configure-mobile-app-android-push-access.md)
>* [Konfigurera push-åtkomst för iOS-mobilappar](configure-mobile-app-ios-push-access.md)

>



