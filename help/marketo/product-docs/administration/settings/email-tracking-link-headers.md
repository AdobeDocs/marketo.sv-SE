---
description: Anpassa länkrubriker för e-postspårning i Admin under E-post, inklusive Strict-Transport-Security för HTTPS, med riktlinjer för IT-granskning.
title: Länkrubriker för e-postspårning
exl-id: 2db1f1b3-3afe-4710-a8b1-b06fbf09ec8c
feature: Administration
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---

# Länkrubriker för e-postspårning {#email-tracking-link-headers}

Följ stegen nedan för att anpassa länkrubrikerna för e-postspårning.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/email-tracking-link-headers-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/email-tracking-link-headers-2.png)

1. Rulla ned till Anpassade rubrikalternativ. Välj önskade inställningar och klicka på **[!UICONTROL Save Changes]**.

   ![](assets/email-tracking-link-headers-3.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Använd det här för att garantera att spårningslänkar alltid serveras via HTTPS (ska endast anges för prenumerationer med spårningslänkar som skyddas av SSL)</td>
 </tr>
</table>

>[!CAUTION]
>
>Det är viktigt att du granskar dessa inställningar med IT-teamet för att avgöra vilken policy din organisation ska ha. Felaktiga inställningar kan hindra vissa besökare från att få åtkomst till dina e-postlänkar.
