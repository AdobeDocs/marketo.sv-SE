---
description: Aktivera/inaktivera anpassad objektsynkronisering - Marketo Docs - produktdokumentation
title: Aktivera/inaktivera synkronisering av anpassat objekt
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Aktivera/inaktivera synkronisering av anpassat objekt {#enable-disable-custom-object-sync}

Egna objekt som skapas i Veeva CRM-instansen kan också ingå i Marketo Engage. Så här konfigurerar du det.

## Aktivera eller inaktivera synkronisering av anpassat objekt {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. I Marketo klickar du på **Administratör** sedan **Veeva Objects Sync**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Om det här är ditt första anpassade objekt klickar du på Synkronisera schema. Om inte, klicka **Uppdatera schema** för att vara säker på att du har de senaste.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Om den globala synkroniseringen körs inaktiverar du den genom att klicka på **Inaktivera global synkronisering**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Det kan ta några minuter att synkronisera det anpassade objektschemat Veeva.

1. Klicka **Uppdatera schema**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Markera det objekt som du vill synkronisera och klicka på Aktivera synkronisering.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo kan bara synkronisera ett anpassat objekt om det har en direkt relation till kontakt- eller kontoobjektet i Veeva CRM.

1. Klicka **Aktivera synkronisering** igen.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Gå tillbaka till fliken Veeva och klicka på **Aktivera synkronisering**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Använda egna objekt {#using-your-custom-objects}

>[!NOTE]
>
>Du kan inte använda anpassade objekt i smarta kampanjer med utlösare.

1. I den smarta listan drar du över filtret&quot;Har möjlighet&quot; och anger det till **True**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Du kan även använda filterbegränsningar för att begränsa fokus.

   ![](assets/enable-disable-custom-object-sync-9.png)

Underbar! Nu kan du använda det här anpassade objektets data i smarta kampanjer och smarta listor.

>[!MORELIKETHIS]
>
>[Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
