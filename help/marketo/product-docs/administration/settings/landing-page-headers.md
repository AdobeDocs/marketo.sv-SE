---
description: Landningssidhuvuden - Marketo Docs - produktdokumentation
title: Landningssidhuvuden
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Landningssidhuvuden {#landing-page-headers}

Följ stegen nedan för att anpassa några av HTTP-rubrikerna i dina domäner för landningssidan.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/landing-page-headers-1.png)

1. Klicka på **[!UICONTROL Landing Pages]**.

   ![](assets/landing-page-headers-2.png)

1. Klicka på **[!UICONTROL Edit]** bredvid HTTP-rubriker för landningssida.

   ![](assets/landing-page-headers-3.png)

1. Välj önskade inställningar och klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Använd det här för att garantera att anslutningar till landningssidor alltid hanteras via HTTPS (ska endast anges för prenumerationer med landningssidor som skyddas av SSL)</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Här kan du ange om värdbaserade Marketo Engage-resurser kan bäddas in på externa webbsidor eller inte</td>
 </tr>
</table>

>[!CAUTION]
>
>Det är viktigt att du granskar dessa inställningar med IT-teamet för att avgöra vilken policy din organisation ska ha. Felaktiga inställningar kan hindra vissa besökare från att komma åt dina landningssidor.
