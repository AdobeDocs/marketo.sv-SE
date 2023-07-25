---
description: Synkronisering av anpassade objekt - Marketo Docs - produktdokumentation
title: Synkronisering av anpassat objekt
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Synkronisering av anpassat objekt {#custom-object-sync}

Egna objekt som skapas i Veeva CRM-instansen kan också ingå i Marketo Engage. Så här konfigurerar du det.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du vill använda ett anpassat objekt måste det associeras med en kontakt eller ett kontoobjekt i Veeva CRM.

## Aktivera anpassat objekt {#enable-custom-object}

1. I Marketo klickar du på **Administratör** sedan **Veeva Objects Sync**.

   ![](assets/custom-object-sync-1.png)

1. Om det här är ditt första anpassade objekt klickar du på **Synkroniseringsschema**.

   ![](assets/custom-object-sync-2.png)

1. Klicka **Inaktivera global synkronisering**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Den inledande synkroniseringen av det anpassade objektschemat Veeva kan ta några minuter.

1. Dra det anpassade objekt som du vill synkronisera till arbetsytan.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Anpassade objekt måste ha unika namn. Marketo stöder inte två olika anpassade objekt med samma namn.

1. Klicka **Aktivera synkronisering**.

   ![](assets/custom-object-sync-5.png)

1. Klicka **Aktivera synkronisering** igen.

   ![](assets/custom-object-sync-6.png)

1. Gå tillbaka till **Veeva** -fliken.

   ![](assets/custom-object-sync-7.png)

1. Klicka **Aktivera synkronisering**.

   ![](assets/custom-object-sync-8.png)

1. Om du vill visa alla anpassade vevevevektorobjekt klickar du på Synkronisera med admin och veva-objekt.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo stöder bara anpassade entiteter som är länkade till standardenheter en till två nivåer djupt.

Underbar! Nu kan du använda data från det här anpassade objektet i Smarta kampanjer och Smarta listor.

>[!MORELIKETHIS]
>
>* [Synkronisera samtal och ringa nyckelmeddelanden](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
