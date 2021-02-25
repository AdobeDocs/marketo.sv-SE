---
unique-page-id: 4720149
description: Implementera RTP i Wordpress - Marketo Docs - produktdokumentation
title: Implementera RTP i Wordpress
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---


# Implementera RTP i Wordpress {#implementing-rtp-on-wordpress}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Öppna filen **header.php** för ditt **WordPress-tema**.

   Du kan antingen använda en FTP-klient för att komma åt servern eller redigera dina temafiler direkt från instrumentpanelen i WordPress. Filredigeraren finns under fliken **Utseende** på sidofältsmenyn.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. I listan med mallfiler till höger om textredigeraren söker du efter **header.php** och öppnar den.

1. Gå till **Kontoinställningar**.

   a. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopiera JavaScript-taggen RTP och klistra in den i webbplatsmallarna.

   a. Kontrollera att det är det första skriptet i sidhuvudet - mellan **`<head> </head>`**-taggarna.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicka på **Uppdatera fil** för header.php-filen.

1. Kontrollera att den visas på alla sidor, inklusive landningssidor och underdomäner.

   a. Du kan göra detta genom att högerklicka på webbplatsens sida. Gå till **Visa sidkälla.** Sök efter  **** RTP för att hitta taggen.
