---
unique-page-id: 4720149
description: Implementera RTP i Wordpress - Marketo Docs - produktdokumentation
title: Implementera RTP i Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Implementerar RTP på [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Följ installationsanvisningarna nedan för att implementera [!UICONTROL RTP tag]:

1. Öppna filen **header.php** för ditt **[!DNL WordPress]-tema**.

   Du kan antingen använda en FTP-klient för att komma åt servern eller redigera dina temafiler direkt från kontrollpanelen [!DNL WordPress]. Filredigeraren finns under fliken **[!UICONTROL Appearance]** på sidofältsmenyn.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. I listan med mallfiler till höger om textredigeraren söker du efter **header.php** och öppnar den.

1. Gå till **[!UICONTROL Account Settings]**.

   a. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Under [!UICONTROL Domain] letar du reda på den relevanta domänen och klickar på **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopiera RTP JavaScript-taggen och klistra in den i webbplatsmallarna.

   a. Kontrollera att det är det första skriptet i sidhuvudet - mellan **`<head> </head>`** -taggarna.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicka på **[!UICONTROL Update File]** för header.php-filen.

1. Kontrollera att den visas på alla sidor, inklusive landningssidor och underdomäner.

   a. Du kan göra detta genom att högerklicka på webbplatsens sida. Gå till **[!UICONTROL View Page Source].** Sök efter **RTP** för att hitta taggen.
