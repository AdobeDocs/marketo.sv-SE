---
unique-page-id: 42762511
description: Konfigurera Adobe Experience Cloud Audience Sharing - Marketo Docs - produktdokumentation
title: Konfigurera Adobe Experience Cloud målgruppsdelning
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: 760e39e662f361831eed63d424b74dc90bbfd2e2
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Konfigurera Adobe Experience Cloud Audience Sharing {#set-up-adobe-experience-cloud-audience-sharing}

Om du vill dela målgruppsdata med dina Adobe-program måste du först ange dina Adobe IMS-organisationsuppgifter i Marketo. Så här gör du.

>[!NOTE]
>
>En HIPAA-klar distribution av en Marketo-instans kan inte använda den här integreringen.

1. Klicka på **Admin** i Marketo.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Klicka på **Organisationsmappning för Adobe** under Integrering.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicka på **Redigera**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Ange ditt Adobe IMS-organisations-ID (läs om hur du hittar [här](https://docs.adobe.com/content/help/en/control-panel/using/faq.html)) och klicka på **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicka på **Bekräfta**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicka på **Stäng**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!NOTE]
   >
   >Av säkerhetsskäl måste du vara organisationsadministratör för den Adobe-organisation som du vill mappa till. Annars misslyckas åtgärden.

1. Om du _inte_ redan är inloggad visas ett popup-fönster på en ny flik/i ett nytt fönster. Logga in på din Adobe-organisation (den här åtgärden validerar organisationsåtkomsten).

Och det är allt! Nu kan du [dela målgruppsdata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md) till eller [synkronisera en målgrupp](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md) från Adobe Experience Cloud.
