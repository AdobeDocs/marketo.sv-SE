---
unique-page-id: 4720149
description: Implementera RTP i Wordpress - Marketo Docs - produktdokumentation
title: Implementera RTP i Wordpress
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Implementera RTP i Wordpress {#implementing-rtp-on-wordpress}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Öppna filen **header.php** i **WordPress-temat**.

   Du kan antingen använda en FTP-klient för att komma åt servern eller redigera dina temafiler direkt från instrumentpanelen i WordPress. Filredigeraren finns under fliken **Utseende** på sidofältsmenyn.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. I listan med mallfiler till höger om textredigeraren söker du efter **header.php** och öppnar den.
1. Gå till **Kontoinställningar.**

   Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopiera JavaScript-taggen RTP och klistra in den i webbplatsmallarna.

   Kontrollera att det är det första skriptet i sidhuvudet - mellan **`<head> </head>`** -taggarna.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicka på **Uppdatera fil** för header.php-filen.
1. Kontrollera att den visas på alla `pages including` landningssidor och underdomäner.

   Du kan göra detta genom att högerklicka på din `website’s` sida. Gå till **Visa sidkälla.** Sök efter **RTP** för att hitta taggen.
