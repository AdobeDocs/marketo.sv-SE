---
unique-page-id: 4720215
description: Implementera RTP på Wordpress Enterprise - Marketo Docs - produktdokumentation
title: Implementera RTP i Wordpress Enterprise
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Implementera RTP på Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Gå till Kontoinställningar för**.**

   1. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 3.\
      ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Kopiera JavaScript-taggen RTP.
1. Logga in på ditt WordPress-konto som Admin User

   1. Under **Utseende** går du till **Eget JavaScript**.
   1. Klistra in RTP Javascript-taggen direkt efter den befintliga koden.

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
