---
unique-page-id: 4720151
description: Implementera RTP på Marketo Landing Pages - Marketo Docs - produktdokumentation
title: Implementera RTP på Marketo-landningssidor
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Implementera RTP på Marketo-landningssidor {#implementing-rtp-on-marketo-landing-pages}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Gå till **Design Studio.** Öppna det objekt som du vill redigera. Välj **Mallåtgärder** och välj **Redigera utkast**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Gör malländringar på fliken **HTML-källa**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Gå till Kontoinställningar** i ditt RTP-konto.**

1. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Kopiera JavaScript-taggen RTP och klistra in den i alla dina startsidmallar mellan **`<head> </head>`**-taggarna.
1. Klicka på **Spara** och **Stäng** fönstret.
1. I **Design Studio** godkänner du landningssidan från **Mallåtgärder** och klickar på **Godkänn**.\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Slutligen måste du **omgodkänna** alla landningssidor som använder den mallen för att malländringarna ska börja gälla. Du kan omgodkänna alla sidor på en gång i huvudsektionen Landing Pages.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Kontrollera att den visas på alla `pages including` landningssidor och underdomäner.

   Du kan göra detta genom att högerklicka på sidan `website’s`. Gå till **Visa sidkälla.** Sök efter  **** RTP för att hitta taggen.
