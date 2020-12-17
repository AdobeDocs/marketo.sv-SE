---
unique-page-id: 2953384
description: Aktivera synkronisering för en anpassad enhet - Marketo Docs - Produktdokumentation
title: Aktivera synkronisering för en anpassad entitet
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Aktivera synkronisering för en anpassad entitet {#enable-sync-for-a-custom-entity}

Om du vill att anpassade entitetsdata från Dynamics ska vara tillgängliga i Marketo, så här aktiverar du synkroniseringen:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till avsnittet **Admin**.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Välj **Microsoft Dynamics** och klicka på **Inaktivera synkronisering**.

   Du måste inaktivera den globala synkroniseringen tillfälligt för att kunna aktivera eller inaktivera en anpassad entitet.
   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Klicka på länken** Dynamics Entities Sync** under Databashantering.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Klicka på länken **Synkronisera schema**.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Markera den enhet som du vill synkronisera och klicka på **Aktivera synkronisering**.

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. Markera de fält som du vill synkronisera eller använda som [begränsningar](../../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) och/eller utlösare i smarta listor. När du är klar klickar du på **Aktivera synkronisering**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >Under synkroniseringsprocessen kan du se att objektet Synkronisera dynamiska entiteter försvinner från navigeringsträdet. Detta beteende förväntas och kommer att visas igen när synkroniseringen är klar.

1. Enheten har nu en grön bockmarkering.

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. Glöm inte att aktivera den globala synkroniseringen igen!

   ![](assets/image2015-11-10-9-3a48-3a35.png)

Absolut! Kraftfulla grejer.
