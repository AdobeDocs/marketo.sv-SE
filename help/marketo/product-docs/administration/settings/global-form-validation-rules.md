---
description: Global Form Validation Rules - Marketo Docs - Product Documentation
title: Valideringsregler för globala formulär
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 1%

---

# Valideringsregler för globala formulär {#global-form-validation-rules}

Med den här funktionen kan du blockera specifika domäner från att skicka till Marketo Engage-formulär.

## Aktivera åtkomst {#how-to-enable-access}

Innan du kan använda den här funktionen måste du aktivera dess behörighet per önskad roll.

1. I Marketo klickar du på **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/global-form-validation-rules-2.png)

1. Klicka på **[!UICONTROL Roles]** -fliken.

   ![](assets/global-form-validation-rules-3.png)

1. Dubbelklicka på den roll du vill ge behörighet till.

   ![](assets/global-form-validation-rules-4.png)

1. Klicka på **+** -signering bredvid Access Admin.

   ![](assets/global-form-validation-rules-5.png)

1. Bläddra nedåt och markera **[!UICONTROL Access Form Validation Rules]** och klicka **[!UICONTROL Save]**.

   ![](assets/global-form-validation-rules-6.png)

## Skapa ny valideringsregel för formulär {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Dessa regler gäller för alla formulär i dina Marketo Engage-prenumerationer.

1. I Marketo klickar du på **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Klicka på **[!UICONTROL Global Form Validation Rule]**.

   ![](assets/global-form-validation-rules-8.png)

1. Klicka på **[!UICONTROL New Form Validation Rule]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >I listrutan Åtgärder för formulärverifieringsregel kan du ta bort eller redigera befintliga regler.

1. Ge regeln ett namn, ge den en valfri beskrivning och skriv felmeddelandet som du vill att formulärbesökarna ska se. Ange den eller de domäner du vill blockera i regelrutan, välj **[!UICONTROL Activate Rule]** och klicka **[!UICONTROL Create]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage har en definierad blockeringslista av kostnadsfria e-postdomäner för konsumenter som blockeras när vår förinlästa regel&quot;Blockeringslista för e-postdomän för konsumenter&quot; används. [Visa listan här](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Inaktivera åtkomst per formulär{#how-to-disable-access-per-form}

När det är aktiverat gäller reglerna alla formulär. Om du har ett formulär med specifika krav och du inte vill att något ska avvisas kan du inaktivera [!UICONTROL Global Form Validation Rules] i formulärinställningarna.

1. Klicka på **[!UICONTROL Form Settings]** sedan **[!UICONTROL Settings]**.

   ![](assets/global-form-validation-rules-11.png)

1. Klicka på **[!UICONTROL Global Form Validation Rules]** nedrullningsbar meny och välj **[!UICONTROL Disabled]**.

   ![](assets/global-form-validation-rules-12.png)

När du godkänner och publicerar formuläret kommer det att ignorera [!UICONTROL Global Form Validation Rules].
