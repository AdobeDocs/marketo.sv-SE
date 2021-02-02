---
unique-page-id: 3571846
description: Microsoft Dynamics Sync -Anpassad entitetssynkronisering - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - anpassad entitetssynkronisering
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Synkronisering av anpassad entitet {#microsoft-dynamics-sync-custom-entity-sync}

Om du behöver aktivera den första anpassade entitetssynkroniseringen för att göra data från Dynamics tillgängliga i Marketo, så här gör du det.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du vill använda ett anpassat objekt måste det vara associerat med ett [lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)-, [kontakt](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)- eller [konto](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)objekt i Dynamics.

>[!CAUTION]
>
>Kontrollera att den första synkroniseringen är slutförd (du meddelas via e-post) innan du börjar synkronisera anpassade entiteter.

1. Gå till avsnittet Admin.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Klicka på **Inaktivera Synkronisera** om du tillfälligt vill inaktivera den globala standardsynkroniseringen.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Installera en version av Microsoft Dynamics som har stöd för anpassad entitetssynkronisering (efter 2_0_0_2). Se [Marketo Plugin Releases for MIcrosoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

1. Ge Marketo Sync User läsåtkomst till alla enheter du tänker synkronisera.

1. Klicka på länken **Synkronisera Dynamics-entiteter** under Databashantering.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Klicka på länken **Synkronisera schema** för att visa listan över tillgängliga anpassade entiteter.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. När listan har synkroniserats markerar du de fält som du vill synkronisera och de som du vill använda som [begränsningar](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) och/eller utlösare i smarta listor. När du är klar klickar du på **Aktivera synkronisering**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. Återaktivera den globala synkroniseringen.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo stöder bara anpassade entiteter som är länkade till standardenheter på en eller två nivåer djupt.

   >[!NOTE]
   >
   >Enhetsnamn får innehålla högst **33 tecken**.

Du är bra!
