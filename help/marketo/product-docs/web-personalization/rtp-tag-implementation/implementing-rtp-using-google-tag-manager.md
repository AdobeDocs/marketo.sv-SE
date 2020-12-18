---
unique-page-id: 4720145
description: Implementera RTP med Google Tag Manager - Marketo Docs - Produktdokumentation
title: Implementera RTP med Google Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 0%

---


# Implementera RTP med Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP `tag please`.

1. Logga in på ditt Google Tag Manager-konto.

1. Lägg till en ny tagg > Taggkonfigurationer > Anpassad HTML-tagg**.** Ring det **RTP**.

1. Logga in på ditt RTP-konto**.**

1. Gå till Kontoinställningar för**.**

   1. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 6.

      ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ** ![](assets/image2014-11-30-15-3a20-3a17.png)

   **

1. Kopiera RTP JavaScript-taggen och klistra in den i den nya **anpassade HTML-taggen** som du skapade (steg 1).

1. Klicka på **+Lägg till regel i Fire Tag**. Välj **Alla sidor**.

1. Klicka på **Spara **och [publicera den nya versionen](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Kontrollera att den visas på alla `pages, including` landningssidor och underdomäner.

   1. Du kan göra detta genom att högerklicka på din `website’s`-sida. Gå till **Inspect Element. **Sök efter **RTP **för att hitta taggen.

