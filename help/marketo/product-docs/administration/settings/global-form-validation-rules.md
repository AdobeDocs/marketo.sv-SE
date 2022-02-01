---
description: Global Form Validation Rules - Marketo Docs - Product Documentation
title: Valideringsregler för globala formulär
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: a3acf82afa894160b20dff76fdd5132a234dfbd3
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Valideringsregler för globala formulär {#global-form-validation-rules}

Med den här funktionen kan du blockera specifika domäner från att skicka till Marketo Engage-formulär.

## Aktivera åtkomst {#how-to-enable-access}

Innan du kan använda den här funktionen måste du aktivera dess behörighet per önskad roll.

1. In Marketo, click **Admin**.

   ![](assets/global-form-validation-rules-1.png)

1. Klicka **Användare och roller**.

   ![](assets/global-form-validation-rules-2.png)

1. Click the **Roles** tab.

   ![](assets/global-form-validation-rules-3.png)

1. Dubbelklicka på den roll du vill ge behörighet till.

   ![](assets/global-form-validation-rules-4.png)

1. Klicka på **+** -signering bredvid Access Admin.

   ![](assets/global-form-validation-rules-5.png)

1. Scroll down and select **Access Form Validation Rules** and click **Save**.

   ![](assets/global-form-validation-rules-6.png)

## Skapa ny valideringsregel för formulär {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Dessa regler gäller för alla formulär i dina Marketo Engage-prenumerationer.

1. In Marketo, click **Admin**.

   ![](assets/global-form-validation-rules-7.png)

1. Klicka **Valideringsregel för globalt formulär**.

   ![](assets/global-form-validation-rules-8.png)

1. Click **New Form Validation Rule**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >The Form Validation Rule Actions drop-down allows you to delete or edit existing rules.

1. Ge regeln ett namn, ge den en valfri beskrivning och skriv felmeddelandet som du vill att formulärbesökarna ska se. Ange den eller de domäner du vill blockera i regelrutan, välj **Aktivera regel** och klicka **Skapa**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage has a defined blocklist of free consumer email domains that are blocked when using our pre-loaded &quot;Consumer Email Domain Blocklist&quot; rule. [View that list here](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).
