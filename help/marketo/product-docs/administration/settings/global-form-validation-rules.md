---
description: Global Form Validation Rules - Marketo Docs - Product Documentation
title: Valideringsregler för globala formulär
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: 2736e8a0456de76b9894312c26f6ba9c0345daee
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Valideringsregler för globala formulär {#global-form-validation-rules}

Med den här funktionen kan du blockera specifika domäner från att skicka till Marketo Engage-formulär.

## Aktivera åtkomst {#how-to-enable-access}

Innan du kan använda den här funktionen måste du aktivera dess behörighet per önskad roll.

1. I Marketo klickar du på **Administratör**.

   ![](assets/global-form-validation-rules-1.png)

1. Klicka **Användare och roller**.

   ![](assets/global-form-validation-rules-2.png)

1. Klicka på **Roller** -fliken.

   ![](assets/global-form-validation-rules-3.png)

1. Dubbelklicka på den roll du vill ge behörighet till.

   ![](assets/global-form-validation-rules-4.png)

1. Klicka på **+** -signering bredvid Access Admin.

   ![](assets/global-form-validation-rules-5.png)

1. Bläddra nedåt och markera **Få åtkomst till verifieringsregler för formulär** och klicka **Spara**.

   ![](assets/global-form-validation-rules-6.png)

## Skapa ny valideringsregel för formulär {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Dessa regler gäller för alla formulär i dina Marketo Engage-prenumerationer.

1. I Marketo klickar du på **Administratör**.

   ![](assets/global-form-validation-rules-7.png)

1. Klicka **Valideringsregel för globalt formulär**.

   ![](assets/global-form-validation-rules-8.png)

1. Klicka **Valideringsregel för nytt formulär**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >I listrutan Åtgärder för formulärverifieringsregel kan du ta bort eller redigera befintliga regler.

1. Ge regeln ett namn, ge den en valfri beskrivning och skriv felmeddelandet som du vill att formulärbesökarna ska se. Ange den eller de domäner du vill blockera i regelrutan, välj **Aktivera regel** och klicka **Skapa**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage har en definierad blockeringslista av kostnadsfria e-postdomäner för konsumenter som blockeras när vår förinlästa regel&quot;Blockeringslista för e-postdomän för konsumenter&quot; används. [Visa listan här](/help/marketo/product-docs/administration/settings/assets/freemaildomains_2023.csv).

## Inaktivera åtkomst per formulär{#how-to-disable-access-per-form}

När det är aktiverat gäller reglerna alla formulär. Om du har ett formulär med specifika krav, och du inte vill ha något avvisat, kan du inaktivera globala regler för formulärvalidering i formulärets inställningar.

1. Klicka på **Formulärinställningar** sedan **Inställningar**.

   ![](assets/global-form-validation-rules-11.png)

1. Klicka på listrutan Valideringsregler för globala formulär och välj **Handikappade**.

   ![](assets/global-form-validation-rules-12.png)

När du godkänner och publicerar formuläret kommer det att ignorera dina globala regler för formulärvalidering.
