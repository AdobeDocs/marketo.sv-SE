---
unique-page-id: 2953384
description: Aktivera synkronisering för en anpassad enhet - Marketo Docs - produktdokumentation
title: Aktivera synkronisering för en anpassad entitet
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Aktivera synkronisering för en anpassad entitet {#enable-sync-for-a-custom-entity}

Om du vill att anpassade entitetsdata från Dynamics ska vara tillgängliga i Marketo Engage, så här aktiverar du synkroniseringen för den.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>* När du aktiverar synkronisering för en anpassad enhet utför Marketo en inledande synkronisering för att hämta alla data för det anpassade objektet.
>* Medlemmar i marknadsföringslista och marknadsföringslista är _stöds inte_ just nu.

>[!IMPORTANT]
>
>Marketo Sync User behöver läsåtkomst till det anpassade objektet för att kunna lista det och synkronisera det.

1. Gå till **[!UICONTROL Admin]** -avsnitt.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Välj **[!UICONTROL Microsoft Dynamics]** och klicka **[!UICONTROL Disable Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Du måste inaktivera den globala synkroniseringen tillfälligt för att kunna aktivera eller inaktivera en anpassad entitet.

1. Klicka på **[!UICONTROL Dynamics Entities Sync]** länk.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Klicka på **[!UICONTROL Sync schema]** länk.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Markera den enhet som du vill synkronisera och klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Markera de fält som du vill synkronisera eller använda som [begränsningar](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} och/eller utlösare i smarta listor. När du är klar klickar du **[!UICONTROL Enable Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Under synkroniseringsprocessen kan du se att[!UICONTROL Dynamic Entities Sync]&quot; försvinner från navigeringsträdet. Detta beteende förväntas och kommer att visas igen när synkroniseringen är klar.

1. Enheten har nu en grön bockmarkering.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Glöm inte att aktivera den globala synkroniseringen igen!

   ![](assets/enable-sync-for-a-custom-entity-8.png)
