---
unique-page-id: 2953384
description: Aktivera synkronisering för en anpassad enhet - Marketo Docs - produktdokumentation
title: Aktivera synkronisering för en anpassad entitet
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: dadaf5bd8e887309d0e9ee8fc25fc58d1c4fbe97
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Aktivera synkronisering för en anpassad entitet {#enable-sync-for-a-custom-entity}

Om du vill att anpassade entitetsdata från Dynamics ska vara tillgängliga i Marketo gör du så här för att aktivera synkroniseringen för den.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>* När du aktiverar synkronisering för en anpassad enhet utför Marketo en inledande synkronisering för att hämta alla data för det anpassade objektet.
>* Medlemmar i marknadsföringslista och marknadsföringslista är **stöds inte** just nu.


1. Gå till **Administratör** -avsnitt.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Välj **Microsoft Dynamics** och klicka **Inaktivera synkronisering**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Du måste inaktivera den globala synkroniseringen tillfälligt för att kunna aktivera eller inaktivera en anpassad entitet.

1. Under Databashantering klickar du på **Synkronisering av Dynamics-entiteter** länk.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Klicka på **Synkroniseringsschema** länk.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Markera den enhet som du vill synkronisera och klicka på **Aktivera synkronisering**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Markera de fält som du vill synkronisera eller använda som [begränsningar](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) och/eller utlösare i smarta listor. När du är klar klickar du på **Aktivera synkronisering**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Under synkroniseringsprocessen kan du märka att objektet Synkronisera dynamiska entiteter försvinner från navigeringsträdet. Detta beteende förväntas och kommer att visas igen när synkroniseringen är klar.

1. Enheten har nu en grön bockmarkering.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Glöm inte att aktivera den globala synkroniseringen igen!

   ![](assets/enable-sync-for-a-custom-entity-8.png)
