---
unique-page-id: 2953132
description: Understanding Batch and Trigger Smart Campaigns - Marketo Docs - Product Documentation
title: Förstå smarta kampanjer i grupp och utlösare
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---


# Förstå smarta kampanjer i grupp och utlösare {#understanding-batch-and-trigger-smart-campaigns}

Det finns två typer av smarta kampanjer: Batch och utlösare.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Batch Smart Campaign {#batch-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>En batchkampanj startas vid en viss tidpunkt och påverkar en viss uppsättning personer på en gång. Ett exempel är att skicka ett e-postmeddelande till alla i Kalifornien.

Smarta gruppkampanjer har bara filter i avsnittet med smarta listor (d.v.s. inga utlösare).

![](assets/batch-filter.png)

Om du klickar på fliken **Schemalägg** visas en bekräftelse på att den smarta kampanjen är inställd på&quot;Gruppera&quot;.

![](assets/batch-c4.png)

**Smarta gruppkampanjer**

* Kan schemaläggas för återkommande aktiviteter, som dagliga, veckovisa och månadsvisa. Du kan också få dem att springa bara en gång.
* Är synliga i [programschemavyn](../../../../product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md).\
   *Observera att inget efter ett &quot;Vänta&quot;-steg i den smarta kampanjen kommer att inkluderas i vyn.

<br> 

## Utlös Smart Campaign {#trigger-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>En utlösande smart kampanj påverkar en person i taget baserat på en utlöst händelse. Ett exempel på en utlösare är att klicka på en länk i ett e-postmeddelande.

Om en smart kampanj använder minst en utlösare i den smarta listsektionen ställs läget automatiskt in på utlösare.

![](assets/trigger.png)

Om du klickar på fliken **Schemalägg** visas en bekräftelse på att den smarta kampanjen är inställd på&quot;Triggered&quot;.

![](assets/trigger2.png)

**Utlös smarta kampanjer**

* Det går inte att schemalägga för återkommande aktiviteter. De kan bara anges som aktiva eller inaktiva.
* Du kan ställa in mer än en utlösare. Om någon utlösare aktiveras körs kampanjåtgärderna.

## Titta på en video om hur du skapar utlösta e-postkampanjer {#watch-a-video-on-creating-triggered-email-campaigns}

`<iframe width="630" height="470" src="//play.vidyard.com/6zNazwTgt2LNeCjPAt3W9K.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

>[!TIP]
>
>Använd [aktivitetsloggen](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) för att se vad som har hänt steg för steg inom smarta kampanjer. Du hittar aktivitetsloggen på den sista fliken på en persons detaljsida.

