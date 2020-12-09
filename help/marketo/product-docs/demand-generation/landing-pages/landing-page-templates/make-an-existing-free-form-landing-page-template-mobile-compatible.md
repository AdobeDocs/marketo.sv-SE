---
unique-page-id: 5472348
description: Gör en befintlig mall för landningssida i friform kompatibel - Marketo Docs - Produktdokumentation
title: Gör en befintlig mall för landningssida i friform kompatibel
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Gör en befintlig mall för landningssida i friform kompatibel {#make-an-existing-free-form-landing-page-template-mobile-compatible}

>[!NOTE]
>
>Mallar för landningssidor som skapades före [januari 2015](../../../../release-notes/2015/release-notes-january-2015.md)måste uppgraderas för att vara mobilkompatibla.

Det kan du göra på två ställen: mallredigeraren och redigeraren för landningssidor.

## Uppgradera från mallredigeraren {#upgrade-from-the-template-editor}

1. Gå till **Design Studio**.

   ![](assets/designstudio-1.png)

1. Välj **Mallar**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Välj en mall där **Mobile Compatible** är **No**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Klicka på **Redigera utkast**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Klicka på **Gör mobilkompatibel**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Klicka på **Uppgradera**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Din landningssidmall är nu mobilkompatibel.

   >[!NOTE]
   >
   >Uppgraderingen bör vara ofarlig, men kontrollera om det finns några skillnader på sidorna. Uppgraderingen kommer att skapa utkast av landningssidor med den mallen.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Vad gör en mall för mobil kompatibel? {#what-makes-a-template-mobile-compatible}

Fantastiska frågor! Mallen måste ha följande taggar:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`  Om allt ser bra ut ser du det här meddelandet.

![](assets/image2015-1-22-20-3a41-3a31.png)

Om något är fel visas ett felmeddelande. Klicka på Reparera för att åtgärda problemet och upprepa valideringsprocessen.

![](assets/image2015-1-22-20-3a43-3a20.png)

Om du gör några ändringar i mallen klickar du på Mallåtgärder och väljer Validera mobilkompatibilitet.

## Uppgradera en mall från sidredigeraren för kostnadsfri landning {#upgrading-a-template-from-the-free-form-landing-page-editor}

När du redigerar en landningssida och klickar på mobilfliken, kommer du ibland att märka att mallen inte har uppgraderats. Rädsla inte! Där kan du uppgradera den.

1. Klicka på fliken **Mobil** .

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Klicka på kryssrutan och klicka på **Aktivera**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >När du aktiverar mobilversionen av en mall skapas utkast för alla landningssidor som använder den.

Häftig! Nu kan du [anpassa mobilvyn](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) för alla dina landningssidor som använder den här mallen.

>[!MORELIKETHIS]
>
>* [Anpassa mobilvyn för din startsida med kostnadsfria formulär](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)

>



