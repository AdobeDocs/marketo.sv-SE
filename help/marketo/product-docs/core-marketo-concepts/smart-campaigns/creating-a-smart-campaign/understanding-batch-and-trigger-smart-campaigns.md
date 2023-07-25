---
unique-page-id: 2953132
description: Understanding Batch and Trigger Smart Campaigns - Marketo Docs - Product Documentation
title: Förstå smarta kampanjer i grupp och utlösare
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Förstå smarta kampanjer i grupp och utlösare {#understanding-batch-and-trigger-smart-campaigns}

Det finns två typer av smarta kampanjer: Batch och utlösare.

## Batch Smart Campaign {#batch-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>En batchkampanj startas vid en viss tidpunkt och påverkar en viss uppsättning personer på en gång. Ett exempel är att skicka ett e-postmeddelande till alla i Kalifornien.

Smarta gruppkampanjer har bara filter i avsnittet med smarta listor (d.v.s. inga utlösare).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Klicka på **Schema** bekräftar att den smarta kampanjen är inställd på&quot;Batch&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Smarta gruppkampanjer**

* Kan schemaläggas för återkommande aktiviteter, som dagliga, veckovisa och månadsvisa. Du kan också få dem att springa bara en gång.
* Är synliga på [programschemavy](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Allt efter ett &quot;Vänta&quot;-steg i den smarta kampanjen inkluderas inte i vyn.

<br> 

## Utlös Smart Campaign {#trigger-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>En utlösande smart kampanj påverkar en person i taget baserat på en utlöst händelse. Ett exempel på en utlösare är att klicka på en länk i ett e-postmeddelande.

Om en smart kampanj använder minst en utlösare i den smarta listsektionen ställs läget automatiskt in på utlösare.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Klicka på **Schema** bekräftar att den smarta kampanjen är inställd på&quot;Triggered&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Utlös smarta kampanjer**

* Det går inte att schemalägga för återkommande aktiviteter. De kan bara anges som aktiva eller inaktiva.
* Du kan ställa in mer än en utlösare. Om någon utlösare aktiveras körs kampanjåtgärderna.

>[!TIP]
>
>Använd [aktivitetslogg](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) för att se vad som hände steg för steg inom smarta kampanjer. Du hittar aktivitetsloggen på den sista fliken på en persons detaljsida.
