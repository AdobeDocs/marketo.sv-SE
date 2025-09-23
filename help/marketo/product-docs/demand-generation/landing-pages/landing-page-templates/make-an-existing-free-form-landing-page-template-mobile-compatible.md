---
unique-page-id: 5472348
description: Gör en befintlig mall för landningssida i friform kompatibel - Marketo Docs - Produktdokumentation
title: Gör en befintlig mall för landningssida i friform kompatibel
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---

# Skapa en befintlig mall för startsida för frihandslayout [!UICONTROL Mobile Compatible] {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Det kan du göra på två ställen: mallredigeraren och redigeraren för landningssidor.

## Uppgradera från mallredigeraren {#upgrade-from-the-template-editor}

1. Gå till **[!UICONTROL Design Studio]**.

   ![](assets/designstudio-1.png)

1. Välj **[!UICONTROL Templates]**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Välj en mall där **[!UICONTROL Mobile Compatible]** är **[!UICONTROL No]**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Klicka på **[!UICONTROL Make Mobile Compatible]**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Klicka på **[!UICONTROL Upgrade]**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Din landningssidmall är nu mobilkompatibel.

   >[!NOTE]
   >
   >Uppgraderingen bör vara ofarlig, men kontrollera om det finns några skillnader på sidorna. Uppgraderingen kommer att skapa utkast av landningssidor med den mallen.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Vad gör en mall [!UICONTROL Mobile Compatible]? {#what-makes-a-template-mobile-compatible}

Fantastiska frågor! Mallen måste ha följande taggar:

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

Om allt ser bra ut ser du det här meddelandet.

![](assets/image2015-1-22-20-3a41-3a31.png)

Om något är fel visas ett felmeddelande. Klicka på Reparera för att åtgärda problemet och upprepa valideringsprocessen.

![](assets/image2015-1-22-20-3a43-3a20.png)

Om du gör några ändringar i mallen klickar du på [!UICONTROL Template Actions] och väljer [!UICONTROL Validate Mobile Compatibility].

## Uppgradera en mall från sidredigeraren för kostnadsfri landning {#upgrading-a-template-from-the-free-form-landing-page-editor}

När du redigerar en landningssida och klickar på mobilfliken, kommer du ibland att märka att mallen inte har uppgraderats. Rädsla inte! Där kan du uppgradera den.

1. Klicka på fliken **[!UICONTROL Mobile]**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Klicka i kryssrutan och klicka på **[!UICONTROL Activate]**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >När du aktiverar mobilversionen av en mall skapas utkast för alla landningssidor som använder den.

Häftig! Du kan nu [anpassa den mobila vyn](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) för alla dina landningssidor som använder den här mallen.
