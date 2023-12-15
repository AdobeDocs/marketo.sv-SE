---
description: Synkronisering av anpassade objekt - Marketo Docs - produktdokumentation
title: Synkronisering av anpassat objekt
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Synkronisering av anpassat objekt {#custom-object-sync}

Egna objekt som skapas i Veeva CRM-instansen kan också ingå i Marketo Engage. Så här ställer du in det.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du vill använda ett anpassat objekt måste det associeras med en kontakt eller ett kontoobjekt i Veeva CRM.

## Aktivera anpassat objekt {#enable-custom-object}

1. Klicka på i Marketo **[!UICONTROL Admin]** sedan **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/custom-object-sync-1.png)

1. Om det här är ditt första anpassade objekt klickar du på **[!UICONTROL Sync Schema]**.

   ![](assets/custom-object-sync-2.png)

1. Klicka på **[!UICONTROL Disable Global Sync]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Den inledande synkroniseringen av det anpassade objektschemat Veeva kan ta några minuter.

1. Dra det anpassade objekt som du vill synkronisera till arbetsytan.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Anpassade objekt måste ha unika namn. Marketo stöder inte två olika anpassade objekt med samma namn.

1. Klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/custom-object-sync-5.png)

1. Klicka **[!UICONTROL Enable Sync]** igen.

   ![](assets/custom-object-sync-6.png)

1. Gå tillbaka till **[!UICONTROL Veeva]** -fliken.

   ![](assets/custom-object-sync-7.png)

1. Klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/custom-object-sync-8.png)

1. Om du vill visa alla anpassade veeva-objekt klickar du på **[!UICONTROL Admin]** och **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo stöder bara anpassade entiteter som är länkade till standardenheter en till två nivåer djupt.

Underbar! Nu kan du använda data från det här anpassade objektet i Smarta kampanjer och Smarta listor.

>[!MORELIKETHIS]
>
>* [Synkronisera samtal och ringa nyckelmeddelanden](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
