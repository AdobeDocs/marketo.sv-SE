---
solution: Marketo Engage
product: marketo
title: Villkorligt innehåll
description: Använd villkorsstyrt innehåll i e-postmeddelanden för att dynamiskt visa innehåll beroende på mottagaren.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 40fdd38d8ec5b63568c8ed9beeab0ef50974b7fd
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Villkorligt innehåll {#conditional-content}

Med villkorligt innehåll kan ni dynamiskt styra vilket innehåll som ska ses av vilken målgrupp. Använd befintliga segment för att bestämma vad en mottagare ser baserat på fördefinierade kriterier.

>[!PREREQUISITES]
>
>Ha minst en segmentering [skapad](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) och [godkänd](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md).

## Lägga till villkorligt innehåll {#add-conditional-content}

1. Öppna det önskade e-postmeddelandet och klicka på **Redigera e-postinnehåll**.

   ![](assets/conditional-content-1.png){width="800" zoomable="yes"}

1. Markera det innehåll som du vill villkora (i det här exemplet väljer vi rubrikbilden). Klicka på ikonen _Aktivera villkorligt innehåll_ .

   ![](assets/conditional-content-2.png)

1. Lådan blir orange. Klicka på ikonen _Välj villkor_ () till vänster för att definiera varianten.

   ![](assets/conditional-content-3.png)

1. Välj önskat segment och klicka på **Markera**.

   ![](assets/conditional-content-4.png)

1. Klicka på ikonen _Redigera bild_ för att ersätta den befintliga bilden för varianten. Välj källa för den nya bilden. I det här exemplet väljer vi biblioteket _Bilder och filer_ i Marketo Engage-prenumerationen.

   ![](assets/conditional-content-5.png)

1. Välj lämplig bild och klicka på **Välj**.

   ![](assets/conditional-content-6.png)

1. Den nya bilden visas. Det är en bra idé att byta namn på varianten så att den blir lättare att identifiera.

   ![](assets/conditional-content-7.png)

1. Om du vill lägga till ytterligare varianter (valfritt) klickar du på **Lägg till variant** och följer samma steg.

   ![](assets/conditional-content-8.png)

1. När du är klar visar varje variant det markerade innehållet.

   ![](assets/conditional-content-9.gif)

1. Mottagarna ser innehåll baserat på de regler som definierats i varje segment. I exemplet ovan ser alla som har &quot;fotboll&quot; i ditt Marketo Engage-fält _Favorite Sport_ fotbollsbilden.

>[!MORELIKETHIS]
>
>* [Definiera segmentregler](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Skapa ett anpassat fält i Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
