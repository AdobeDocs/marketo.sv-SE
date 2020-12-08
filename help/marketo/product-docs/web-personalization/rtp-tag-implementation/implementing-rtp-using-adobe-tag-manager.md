---
unique-page-id: 4720218
description: Implementera RTP med Adobe Tag Manager - Marketo Docs - produktdokumentation
title: Implementera RTP med Adobe Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Implementera RTP med Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Logga in på ditt RTP-konto.
1. Gå till **Kontoinställningar.**

   Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Logga in på ditt Dynamic Tag Manager-konto ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).
1. Gå till **instrumentpanelen.** Klicka på den relevanta webbegenskapen.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Gå till **Regler och** klicka på **Skapa ny regel.**

1. Fyll i följande

   1. Namn: **Marketo RTP**
   1. Villkor (komprimera): Utlösarregel vid - **sidans överkant**
   1. JavaScript (komprimera): klicka på **Lägg till nytt skript**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Anropa den nya taggen: **Marketo RTP-tagg**
1. Ta bort följande kod från RTP-taggen

   * `<script type='text/javascript'>`
   * `</script>`

1. Klistra in JavaScript-taggen RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Se till att du tar bort alla taggar och bara låter skriptet vara (nej `<script type='text/javascript'>` , `</script>` )

1. Klicka på **Spara kod** i skriptredigeraren och **Spara regel** i regelredigeraren.

1. Leta reda på inläsningsregeln för sidan Marketo RTP på panelen Regler och välj **Aktivera regler** i listrutan **Åtgärder**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Kontrollera** att den visas på alla sidor, inklusive landningssidor och underdomäner.

   Du kan göra det genom att högerklicka på webbplatsens sidor. Gå till **Inspect Element**, klicka på **Nätverk, **Sök: **RTP**.
