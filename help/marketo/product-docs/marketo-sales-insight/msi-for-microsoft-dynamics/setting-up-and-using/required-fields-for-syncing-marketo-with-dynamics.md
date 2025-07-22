---
unique-page-id: 11375827
description: Obligatoriska fält för synkronisering av Marketo med Dynamics - Marketo Docs - produktdokumentation
title: Obligatoriska fält för synkronisering av Marketo med Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 1%

---

# Obligatoriska fält för synkronisering av Marketo med [!DNL Dynamics] {#required-fields-for-syncing-marketo-with-dynamics}

Dessa fält *måste* synkroniseras med Marketo för både [!UICONTROL Lead] och för [!UICONTROL Contact] för [!DNL Sales Insight] att fungera:

* Prioritet
* Akut
* Relativa poäng

Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Kontrollera i instansen att fälten är synkroniserade för både **[!UICONTROL Lead]** och **[!UICONTROL Contact]** för att åtgärda detta. Om inte, lägg till dem.

Så här verifierar och lägger du till synkroniseringsfält.

1. Gå till [!UICONTROL Admin] och klicka på **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **[!UICONTROL Edit]** på [!UICONTROL Field Sync Details].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Markera kryssrutan [!UICONTROL Lead] under [!UICONTROL Priority].

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Bläddra nedåt och markera kryssrutan [!UICONTROL Urgency]...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...och kryssrutan [!UICONTROL Relative Score].

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Markera sedan kryssrutorna för [!UICONTROL Priority], [!UICONTROL Urgency] och [!UICONTROL Relative Score] för [!UICONTROL Contact].

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Vänta minst 10 minuter på att en synkronisering ska köras innan du verifierar att du har åtgärdat problemet.

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
