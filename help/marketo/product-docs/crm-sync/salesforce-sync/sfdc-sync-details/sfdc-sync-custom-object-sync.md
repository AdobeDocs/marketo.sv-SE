---
unique-page-id: 2953471
description: SFDC Sync - Sync Custom Object Sync - Marketo Docs - produktdokumentation
title: SFDC Sync - anpassad objektsynkronisering
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---

# SFDC Sync: Anpassad objektsynkronisering {#sfdc-sync-custom-object-sync}

Anpassade objekt som skapas i din [!DNL Salesforce]-instans kan också ingå i Marketo.  Så här ställer du in det.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du vill använda ett anpassat objekt måste det vara associerat med ett [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)-, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)- eller [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) -objekt i [!DNL Salesforce].

>[!IMPORTANT]
>
>Marketo Sync User behöver läsåtkomst till det anpassade objektet för att kunna lista det och synkronisera det.

## Aktivera anpassat objekt  {#enable-custom-object}

1. Klicka på **[!UICONTROL Admin]** och på länken **[!UICONTROL Salesforce Objects Sync]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Om det här är ditt första anpassade objekt klickar du på **[!UICONTROL Sync Schema]**.

   ![](assets/rtaimage-2.png)

1. Klicka på **[!UICONTROL Disable Global Sync]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >En inledande synkronisering av det anpassade objektschemat [!DNL Salesforce] kan ta några minuter.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Dra det anpassade objekt som du vill synkronisera till arbetsytan.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Anpassade objekt måste ha unika namn. Marketo stöder inte två olika anpassade objekt med samma namn.

1. Klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicka på **[!UICONTROL Enable Sync]** igen.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Glöm inte att aktivera den globala synkroniseringen igen!

1. Gå tillbaka till fliken **[!UICONTROL Salesforce]**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Om du vill visa alla dina [!DNL Salesforce] anpassade objekt klickar du på **[!UICONTROL Admin]** och på länken **[!UICONTROL Salesforce Objects Sync]** (samma som steg 1 ovan).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* Marketo stöder bara anpassade entiteter som är länkade till standardenheter på en eller två nivåer.
   >
   >* Det anpassade objektträdet kan visa samma objekt flera gånger på grund av dess direkta anslutningar till ett av huvudobjekten (t.ex. leads, kontakter eller konton eller indirekta anslutningar via ett mellanliggande objekt). I så fall väljer du det objekt som ligger närmast huvudobjektet och väljer bara ett. Om du väljer samma objekt flera gånger kan det försvåra synkroniseringen av det anpassade objektet.

### What&#39;s Next: {#whats-next}

[Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Underbar! Nu kan du använda data från det här anpassade objektet i smarta kampanjer och smarta listor.
