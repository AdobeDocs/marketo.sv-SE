---
unique-page-id: 42762511
description: Konfigurera organisationsmappning för Adobe - Marketo Docs - produktdokumentation
title: Ställ in organisationsmappning för Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# Ställ in organisationsmappning för Adobe {#set-up-adobe-organization-mapping}

För att kunna synkronisera med Adobe-program som Audience Manager, B2B CDP Marketo-kopplingen, [!DNL Dynamic Chat] osv. måste du först ange dina Adobe IMS-organisationsuppgifter i Marketo Engage.

>[!NOTE]
>
>* En HIPAA-klar distribution av en Marketo-instans kan inte använda den här integreringen.
>* För att integreringen ska fungera måste Marketo och dina andra Adobe-program finnas i samma organisation.

>[!IMPORTANT]
>
>För dem som uppgraderar till Adobe Business Platform och Identity Management System fylls det Org ID som är kopplat till prenumerationen redan i och är ett skrivskyddat fält. Stegen i den här artikeln är därför inte tillämpliga.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Klicka på **[!UICONTROL Adobe Organization Mapping]** under Integrering.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Ange ditt Adobe IMS-organisations-ID (läs om hur du hittar [här](https://experienceleague.adobe.com/docs/control-panel/using/faq.html?lang=sv-SE){target="_blank"}) och klicka på **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Klicka på **[!UICONTROL Confirm]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Klicka på **[!UICONTROL Close]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Av säkerhetsskäl måste du vara organisationsadministratör för den Adobe-organisation som du vill mappa till. Annars misslyckas åtgärden. Dessutom måste Adobe-användaren och Marketo-användaren använda samma e-postadress när de loggar in.

1. Om du _inte_ redan är inloggad visas ett popup-fönster på en ny flik/i ett nytt fönster. Logga in på din Adobe-organisation (den här åtgärden validerar organisationsåtkomsten).

Och det är allt! Du kan nu [dela målgruppsdata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} till, eller [synkronisera en målgrupp](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} från Adobe Experience Cloud.
