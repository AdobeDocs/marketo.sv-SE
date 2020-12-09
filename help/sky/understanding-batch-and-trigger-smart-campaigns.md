---
title: understanding-batch-and-trigger-smart-campaign
description: Förstå smarta kampanjer i grupp och utlösare
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Förstå smarta kampanjer i grupp och utlösare

<br> 

Det finns två typer av smarta kampanjer: Batch och utlösare.

## Batch Smart Campaign

En batchkampanj startas vid en viss tidpunkt och påverkar en viss uppsättning personer på en gång. Ett exempel är att skicka ett e-postmeddelande till alla i din databas som bor i Kalifornien.

Smarta gruppkampanjer har bara filter i avsnittet med smarta listor (d.v.s. inga utlösare).

![Bild ett](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Om du klickar på **[!UICONTROL Schedule]** fliken bekräftar du att den smarta kampanjen är inställd på&quot;Gruppera&quot;.

![Bild två](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Smarta gruppkampanjer**

* Kan schemaläggas för återkommande aktiviteter, som dagliga, veckovisa och månadsvisa. Du kan också få dem att springa bara en gång.
* Är synliga i [programschemavyn](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View).
* Allt efter ett &quot;Vänta&quot;-steg i den smarta kampanjen inkluderas inte i vyn.

## Utlös Smart Campaign

En utlösande smart kampanj påverkar en person i taget baserat på en utlöst händelse. Ett exempel på en utlösare är att klicka på en länk i ett e-postmeddelande.

Om en smart kampanj använder minst en utlösare i den smarta listsektionen ställs läget automatiskt in på utlösare.

![Bild tre](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Om du klickar på **[!UICONTROL Schedule]** fliken bekräftar du att den smarta kampanjen är inställd på&quot;Utlösare&quot;.

![Bild fyra](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Utlös smarta kampanjer**

* Det går inte att schemalägga för återkommande aktiviteter. De kan bara anges som aktiva eller inaktiva.
* Du kan ställa in mer än en utlösare. Om _någon_ utlösare utlöses körs kampanjåtgärderna.

>[!TIP]
>
>Använd [aktivitetsloggen](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) för att se vad som har hänt steg för steg inom smarta kampanjer. Du hittar aktivitetsloggen på den sista fliken på en persons detaljsida.
