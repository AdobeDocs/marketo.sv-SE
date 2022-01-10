---
description: Landningssidhuvuden - Marketo Docs - produktdokumentation
title: Landningssidhuvuden
hide: true
hidefromtoc: true
source-git-commit: 921c3279b53bc18ac753b1e3f0672a70fe11abe7
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Landningssidhuvuden {#landing-page-headers}

Följ stegen nedan för att anpassa några av HTTP-rubrikerna i dina domäner för landningssidan.

1. I Marketo klickar du på **Administratör**.

   ![](assets/landing-page-headers-1.png)

1. Klicka **Landningssidor**.

   ![](assets/landing-page-headers-2.png)

1. Klicka **Redigera** intill Landing Page HTTP Headers.

   ![](assets/landing-page-headers-3.png)

1. Välj önskade inställningar och klicka på **Spara** när det är klart.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Använd det här för att garantera att anslutningar till landningssidor alltid hanteras via HTTPS (ska endast anges för prenumerationer med landningssidor som skyddas av SSL)</td>
 </tr>
 <tr>
  <td><strong>X-frame-options</strong></td>
  <td>Här kan du ange om värdbaserade resurser i Marketo Engage kan bäddas in på externa webbsidor eller inte</td>
 </tr>
</table>

>[!CAUTION]
>
>Det är viktigt att du granskar dessa inställningar med IT-teamet för att avgöra vilken policy din organisation ska ha. Felaktiga inställningar kan hindra vissa besökare från att komma åt dina landningssidor.
