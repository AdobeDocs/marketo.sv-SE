---
unique-page-id: 4720145
description: Implementera RTP med Google Tag Manager - Marketo Docs - produktdokumentation
title: Implementera RTP med Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Implementera RTP med Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP-taggen.

1. Logga in på ditt Google Tag Manager-konto.

1. Lägg till en ny tagg > Taggkonfigurationer > Egen HTML-tagg**.** Anropa **RTP**.

1. Logga in på ditt RTP-konto**.**

1. Gå till **Kontoinställningar**.

   a. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Kopiera RTP JavaScript-taggen och klistra in den i den nya **anpassade HTML-taggen** som du skapade (steg 1).

1. Klicka på **+Lägg till regel i Fire Tag**. Välj **Alla sidor**.

1. Klicka på **Spara** och [publicera den nya versionen](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Kontrollera att den visas på alla sidor, inklusive landningssidor och underdomäner.

   a. Du kan göra detta genom att högerklicka på webbplatsens sida. Gå till **Inspect Element** och sök efter **RTP** för att hitta taggen.
