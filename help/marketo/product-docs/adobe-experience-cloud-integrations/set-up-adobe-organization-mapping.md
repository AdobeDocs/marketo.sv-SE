---
unique-page-id: 42762511
description: Konfigurera organisationsmappning för Adobe - Marketo Docs - produktdokumentation
title: Ställ in organisationsmappning för Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: dd4fb7dfc92580c58da70d603b6d92bd8f64493c
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 1%

---

# Ställ in organisationsmappning för Adobe {#set-up-adobe-organization-mapping}

För att kunna synkronisera med Adobe-applikationer som Audience Manager, B2B CDP Marketo-kontakten, [!DNL Dynamic Chat]måste du först ange dina Adobe IMS-organisationsuppgifter i Marketo.

>[!NOTE]
>
>En HIPAA-klar distribution av en Marketo-instans kan inte använda den här integreringen.

>[!CAUTION]
>
>För kunder som har anslutit sig till Adobe Business Platform och Identity Management System fylls det Org-ID som är kopplat till prenumerationen redan i och är ett skrivskyddat fält.

1. I Marketo klickar du på **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Under Integrering klickar du på **[!UICONTROL Adobe Organization Mapping]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Ange ditt Adobe IMS-organisations-ID (läs hur du hittar det [här](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) och klicka på **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicka på **[!UICONTROL Confirm]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicka på **[!UICONTROL Close]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Av säkerhetsskäl måste du vara organisationsadministratör för den Adobe-organisation som du vill mappa till. Annars misslyckas åtgärden. Dessutom måste Adobe-användaren och Marketo-användaren använda samma e-postadress när de loggar in.

1. Om du är _not_ redan inloggad visas ett popup-fönster på en ny flik eller i ett nytt fönster. Logga in på din Adobe-organisation (den här åtgärden validerar organisationsåtkomsten).

Och det är allt! Nu kan du [dela målgruppsdata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} to, or [sync an audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} från Adobe Experience Cloud.
