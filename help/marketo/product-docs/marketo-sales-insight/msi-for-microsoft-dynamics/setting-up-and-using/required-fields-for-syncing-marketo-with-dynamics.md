---
unique-page-id: 11375827
description: Obligatoriska fält för synkronisering av Marketo med Dynamics - Marketo Docs - Produktdokumentation
title: Obligatoriska fält för synkronisering av Marketo med Dynamics
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Obligatoriska fält för synkronisering av Marketo med Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Dessa fält *måste* synkroniseras med Marketo för både lead och för att Kontakt för Sales Insight ska fungera:

* Prioritet
* Akut
* Relativa poäng

Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de fält som saknas. Kontrollera i instansen att fälten är synkroniserade för både **lead** och **kontakt** för att åtgärda detta. Om inte, lägg till dem.

Så här verifierar och lägger du till synkroniseringsfält.

1. Gå till Admin och klicka på Microsoft Dynamics.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på Redigera i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Markera kryssrutan Prioritet under Lead.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Bläddra nedåt och markera kryssrutan Behöver...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...och kryssrutan Relativ poäng.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Markera sedan kryssrutorna Prioritet, Nödvändig och Relativ poäng för kontakt.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Klicka på Spara.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Vänta minst 10 minuter på att en synkronisering ska köras innan du verifierar att du har åtgärdat problemet.

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Stjärnor och flamma för lead-/kontaktposter](http://docs.marketo.com/x/BICMAg)

