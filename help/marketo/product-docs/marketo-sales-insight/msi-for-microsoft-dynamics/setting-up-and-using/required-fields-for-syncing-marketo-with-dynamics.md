---
unique-page-id: 11375827
description: Obligatoriska fält för synkronisering av Marketo med Dynamics - Marketo Docs - produktdokumentation
title: Obligatoriska fält för synkronisering av Marketo med Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Obligatoriska fält för synkronisering av Marketo med Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Dessa fält *måste* synkas med Marketo för både Lead och Contact for Sales Insight:

* Prioritet
* Akut
* Relativa poäng

Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Kontrollera i instansen att fälten är synkroniserade för båda för att åtgärda detta **Lead** och **Kontakt**. Om inte, lägg till dem.

Så här verifierar och lägger du till synkroniseringsfält.

1. Gå till Admin och klicka på **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka **Redigera** i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Markera kryssrutan Prioritet under Lead.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Bläddra nedåt och markera kryssrutan Behöver...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...och kryssrutan Relativ poäng.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Markera sedan kryssrutorna Prioritet, Nödvändig och Relativ poäng för kontakt.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Klicka **Spara**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Vänta minst 10 minuter på att en synkronisering ska köras innan du verifierar att du har åtgärdat problemet.

>[!MORELIKETHIS]
>
>[Stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
