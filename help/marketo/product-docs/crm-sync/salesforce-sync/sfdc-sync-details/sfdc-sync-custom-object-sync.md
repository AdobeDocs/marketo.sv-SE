---
unique-page-id: 2953471
description: SFDC Sync -Custom Object Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Anpassad objektsynkronisering
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# SFDC-synkronisering: Synkronisering av anpassat objekt {#sfdc-sync-custom-object-sync}

Anpassade objekt som skapas i Salesforce-instansen kan också ingå i Marketo.  Så här ställer du in det.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du vill använda ett anpassat objekt måste det associeras med ett [lead](sfdc-sync-lead-sync.md)-, [](sfdc-sync-contact-sync.md)kontaktarkonto [](sfdc-sync-account-sync.md)i Salesforce.

## Aktivera anpassat objekt  {#enable-custom-object}

1. Klicka på **Admin** och **länken** Synkronisera Salesforce-objekt.**

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Om det här är ditt första anpassade objekt klickar du på **Synkronisera schema.**

   ![](assets/rtaimage-2.png)

1. Klicka på **Inaktivera global synkronisering.**

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >En inledande synkronisering av det anpassade Salesforce-objektschemat kan ta några minuter.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Dra det anpassade objekt som du vill synkronisera till arbetsytan.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Anpassade objekt måste ha unika namn. Marketo stöder inte två olika anpassade objekt med samma namn.

1. Klicka på **Aktivera synkronisering.**

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicka på **Aktivera synkronisering** igen.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Glöm inte att aktivera den globala synkroniseringen igen!

1. Gå tillbaka till fliken **Salesforce **.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicka på **Aktivera synkronisering.**

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Om du vill visa alla dina anpassade Salesforce-objekt klickar du på **Admin** och länken** Salesforce-objektsynkronisering **(samma som steg 1 ovan).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo stöder bara anpassade entiteter som är länkade till standardenheter på en eller två nivåer djupt.

### What&#39;s Next: {#whats-next}

[Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Underbar! Nu kan du använda data från det här anpassade objektet i smarta kampanjer och smarta listor.

