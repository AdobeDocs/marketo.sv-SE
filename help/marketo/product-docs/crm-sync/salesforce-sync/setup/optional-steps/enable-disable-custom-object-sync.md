---
unique-page-id: 4719297
description: Aktivera/inaktivera anpassad objektsynkronisering - Marketo Docs - produktdokumentation
title: Aktivera/inaktivera synkronisering av anpassat objekt
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Aktivera/inaktivera synkronisering av anpassat objekt {#enable-disable-custom-object-sync}

Egna objekt som skapas i din Salesforce-instans kan också ingå i Marketo Engage. Så här ställer du in det.

## Aktivera/inaktivera synkronisering av anpassat objekt {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Klicka på **[!UICONTROL Salesforce Objects Sync]** på menyn Databashantering.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Om det här är ditt första anpassade objekt klickar du på **[!UICONTROL Sync schema]**. Klicka annars på **[!UICONTROL Refresh Schema]** för att kontrollera att du har den senaste.

   ![](assets/enable-disable-custom-object-sync-3.png)

1. Om din globala synkronisering körs måste du inaktivera den genom att klicka på **[!UICONTROL Disable Global Sync]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Det kan ta några minuter att synkronisera det anpassade objektschemat [!DNL Salesforce].

1. Klicka på **[!UICONTROL Refresh Schema]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Markera det objekt som du vill synkronisera och klicka på **[!UICONTROL Enable Sync]**.

   >[!TIP]
   >
   >Marketo kan bara synkronisera ett anpassat objekt om det har en direkt relation till lead-, kontakt- eller kontoobjektet i [!DNL Salesforce].

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Klicka på **[!UICONTROL Enable Sync]** igen.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Gå tillbaka till fliken **[!DNL Salesforce]** och klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Använda egna objekt {#using-your-custom-objects}

>[!NOTE]
>
>Du kan inte använda anpassade objekt i smarta kampanjer med utlösare.

1. Dra över filtret **[!UICONTROL Has Opportunity]** i din smarta lista och ange **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Använd sedan filterbegränsningar för att begränsa fokus.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Underbar! Nu kan du använda det här anpassade objektets data i Smarta kampanjer och Smarta listor.

>[!MORELIKETHIS]
>
>[Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
