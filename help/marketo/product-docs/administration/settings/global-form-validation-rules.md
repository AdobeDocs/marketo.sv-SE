---
description: Global Form Validation Rules - Marketo Docs - Product Documentation
title: Valideringsregler för globala formulär
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 1%

---

# Valideringsregler för globala formulär {#global-form-validation-rules}

Med den här funktionen kan du blockera specifika domäner från att skicka till Marketo Engage-formulär.

## Aktivera åtkomst {#how-to-enable-access}

Innan du kan använda den här funktionen måste du aktivera dess behörighet per önskad roll.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/global-form-validation-rules-1.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/global-form-validation-rules-2.png)

1. Klicka på fliken **[!UICONTROL Roles]**.

   ![](assets/global-form-validation-rules-3.png)

1. Dubbelklicka på den roll du vill ge behörighet till.

   ![](assets/global-form-validation-rules-4.png)

1. Klicka på **+** bredvid Åtkomstadministratör.

   ![](assets/global-form-validation-rules-5.png)

1. Rulla ned, markera **[!UICONTROL Access Form Validation Rules]** och klicka på **[!UICONTROL Save]**.

   ![](assets/global-form-validation-rules-6.png)

## Skapa ny valideringsregel för formulär {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Dessa regler gäller för alla formulär i dina Marketo Engage-prenumerationer.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/global-form-validation-rules-7.png)

1. Klicka på **[!UICONTROL Global Form Validation Rule]**.

   ![](assets/global-form-validation-rules-8.png)

1. Klicka på **[!UICONTROL New Form Validation Rule]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >I listrutan Åtgärder för formulärverifieringsregel kan du ta bort eller redigera befintliga regler.

1. Ge regeln ett namn, ge den en valfri beskrivning och skriv felmeddelandet som du vill att formulärbesökarna ska se. Ange de domäner du vill blockera i regelrutan, markera **[!UICONTROL Activate Rule]** och klicka på **[!UICONTROL Create]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage har en definierad blockeringslista av kostnadsfria e-postdomäner för konsumenter som blockeras när vår förinlästa regel&quot;Blockeringslista för e-postdomän för konsumenter&quot; används. [Visa den listan här](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Inaktivera åtkomst per formulär{#how-to-disable-access-per-form}

När det är aktiverat gäller reglerna alla formulär. Om du har ett formulär med specifika krav, och du inte vill ha något avvisat, kan du inaktivera [!UICONTROL Global Form Validation Rules] i formulärets inställningar.

1. Klicka på **[!UICONTROL Form Settings]** och sedan på **[!UICONTROL Settings]** i önskat formulär.

   ![](assets/global-form-validation-rules-11.png)

1. Klicka på listrutan **[!UICONTROL Global Form Validation Rules]** och välj **[!UICONTROL Disabled]**.

   ![](assets/global-form-validation-rules-12.png)

När du godkänner och publicerar formuläret kommer det att ignorera din [!UICONTROL Global Form Validation Rules].
