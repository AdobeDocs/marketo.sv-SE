---
unique-page-id: 4720215
description: Implementera RTP på Wordpress Enterprise - Marketo Docs - produktdokumentation
title: Implementera RTP i Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Implementera RTP i Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Gå till **Kontoinställningar**.

   a. Om du redan har fått din JavaScript-tagg från supporten fortsätter du till steg 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Kopiera RTP JavaScript-taggen.

1. Logga in på ditt WordPress-konto som administratör

   a. Gå till **Anpassad JavaScript** under **Utseende**.
b. Klistra in RTP Javascript-taggen direkt efter den befintliga koden.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >När du klistrar in koden EXCLUDE följande taggar:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Infoga bara själva skriptet.

1. Klicka på **Uppdatera**.
