---
unique-page-id: 7512252
description: Lägg till en mobilapp - Marketo Docs - produktdokumentation
title: Lägg till en mobilapp
exl-id: 79edf8cb-4d8b-440a-aa8a-6ead1a93b95a
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 2%

---

# Lägg till en mobilapp {#add-a-mobile-app}

Skicka push-meddelanden till kundbasen genom att ansluta mobilappen till Marketo.

Appar startar normalt ut i en sandlådemiljö, där inledande utveckling och testning utförs. Utvecklarna använder sedan en produktionsmiljö för att bygga den slutliga app som ska användas av kunderna. Du måste välja lämpligt meddelandecertifikat när du lägger till en mobilapp (se steg 4 nedan).

>[!AVAILABILITY]
>
>
>Alla Marketo Engage-användare har inte köpt den här funktionen. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/image2015-4-22-16-3a12-3a32.png)

1. Klicka på **[!UICONTROL Mobile Apps & Devices]**.

   ![](assets/image2016-1-12-15-3a42-3a30.png)

1. Klicka på **[!UICONTROL New Mobile App]**.

   ![](assets/image2015-4-22-16-3a17-3a15.png)

1. Ange ett namn. I listrutan **[!UICONTROL Type]** väljer du vilken typ av miljö du använder -[!UICONTROL Sandbox] eller [!UICONTROL Production]. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-11-18-15-3a52-3a15.png)

   >[!NOTE]
   >
   >Vi rekommenderar att du använder ett [!UICONTROL Production]-meddelandecertifikat i en [!UICONTROL Production]-miljö. Ett [!UICONTROL Sandbox]-certifikat kommer att installeras i en [!UICONTROL Production]-miljö utan problem, men du kommer inte att få några meddelanden. Om du har frågor om din miljö eller ditt meddelandecertifikat kontaktar du Marketo Admin eller Mobile Apps Developer.

   Snyggt! Nu ska vi konfigurera appen så att den fungerar med Android- och iOS-enheter.

>[!MORELIKETHIS]
>
>* [Konfigurera Android Push Access för mobilappar](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md)
>* [Konfigurera iOS Push Access för mobilappar](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)
