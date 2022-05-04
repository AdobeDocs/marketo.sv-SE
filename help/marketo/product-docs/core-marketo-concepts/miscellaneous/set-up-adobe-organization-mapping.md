---
unique-page-id: 42762511
description: Konfigurera organisationsmappning för Adobe - Marketo Docs - produktdokumentation
title: Ställ in organisationsmappning för Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: db91b204ab13d47e500b1942ca14a3b1f010749c
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Ställ in organisationsmappning för Adobe {#set-up-adobe-organization-mapping}

För att kunna synkronisera med Adobe-program som Audience Manager, B2B CDP Marketo-kontakten, Dynamic Chat osv. måste du först ange dina Adobe IMS Org-uppgifter i Marketo.

>[!NOTE]
>
>En HIPAA-klar distribution av en Marketo-instans kan inte använda den här integreringen.

1. I Marketo klickar du på **Administratör**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Under Integrering klickar du på **Organisationsmappning för Adobe**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicka **Redigera**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Ange ditt Adobe IMS-organisations-ID (läs hur du hittar det [här](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) och klicka på **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicka **Bekräfta**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicka **Stäng**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!NOTE]
   >
   >Av säkerhetsskäl måste du vara organisationsadministratör för den Adobe-organisation som du vill mappa till. Annars misslyckas åtgärden.

1. Om du är _not_ redan inloggad visas ett popup-fönster på en ny flik eller i ett nytt fönster. Logga in på din Adobe-organisation (den här åtgärden validerar organisationsåtkomsten).

Och det är allt! Nu kan du [dela målgruppsdata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;} till eller [synka en målgrupp](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md){target=&quot;_blank&quot;} från Adobe Experience Cloud.
