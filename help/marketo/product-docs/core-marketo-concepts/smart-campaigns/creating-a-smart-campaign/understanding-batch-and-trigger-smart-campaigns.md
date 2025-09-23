---
unique-page-id: 2953132
description: Understanding Batch and Trigger Smart Campaigns - Marketo Docs - Product Documentation
title: Förstå smarta kampanjer i grupp och utlösare
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Förstå smarta kampanjer i grupp och utlösare {#understanding-batch-and-trigger-smart-campaigns}

Det finns två typer av smarta kampanjer: Batch och Trigger.

## Gruppkampanj {#batch-campaign}

>[!NOTE]
>
>**Definition**
>
>En batchkampanj startar vid en viss tidpunkt och påverkar en viss uppsättning personer på en gång. Ett exempel är att skicka ett mejl till alla i Kalifornien.

Batchkampanjer har bara filter i det smarta listavsnittet (dvs. inga utlösare).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Om du klickar på fliken **[!UICONTROL Schedule]** bekräftar du att den smarta kampanjen är inställd på Gruppera.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Batchsmarta kampanjer**

* Kan schemaläggas för återkommande aktiviteter, som dagliga, veckovisa och månadsvisa. Du kan också få dem att springa bara en gång.
* Är synliga i [programschemavyn](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}. Allt efter ett &quot;Vänta&quot;-steg i den smarta kampanjen inkluderas inte i vyn.

<br> 

## Utlös kampanj {#trigger-campaign}

>[!NOTE]
>
>**Definition**
>
>En utlösarkampanj påverkar en person i taget baserat på en utlöst händelse. Ett exempel på en utlösare är att klicka på en länk i ett e-postmeddelande.

Om en smart kampanj använder minst en utlösare i avsnittet Smart lista ställs läget automatiskt in på utlösare.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Om du klickar på fliken **[!UICONTROL Schedule]** bekräftar du att den smarta kampanjen är inställd på&quot;Triggered&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Utlös kampanjer**

* Det går inte att schemalägga för återkommande aktiviteter. De kan bara anges som aktiva eller inaktiva.
* Du kan ställa in mer än en utlösare. Om någon utlösare utlöses körs kampanjåtgärderna.

>[!TIP]
>
>Använd [aktivitetsloggen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} för att se vad som hände steg för steg i dina smarta kampanjer. Du hittar aktivitetsloggen på den sista fliken på en persons detaljsida.
