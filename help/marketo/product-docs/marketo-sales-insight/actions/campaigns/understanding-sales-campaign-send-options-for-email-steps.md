---
description: Förstå alternativ för att skicka säljkampanjer via e-post - Marketo Docs - produktdokumentation
title: Om sändningsalternativ för försäljningskampanj för e-poststeg
hide: true
hidefromtoc: true
source-git-commit: 468488010259c5d81cccf741db5cc4b98d20d9ea
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Om sändningsalternativ för försäljningskampanj för e-poststeg {#understanding-sales-campaign-send-options-for-email-steps}

När du skapar en kampanj har du flera alternativ för hur e-poststegen skapas i Sales Insight Actions. Och beroende på var e-postmeddelandet hamnar i din kampanj skiljer sig även alternativen åt.

Om det är ditt första steg och den första dagen i din kampanj har du följande alternativ:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

Jag väljer när det här e-postmeddelandet ska skickas

* Med det här alternativet kan du välja&quot;skicka vid&quot;-tid för det första e-postmeddelandet i din kampanj när du startar kampanjen genom att lägga till personer.

Skicka det här e-postmeddelandet vid följande tidpunkt

* När ni får igång er kampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny sändningstid när du stänger av din kampanj.

Skapa en uppgift; Jag skickar det här e-postmeddelandet själv

* Med det här alternativet skapas en e-postaktivitet (och synkroniseras med Salesforce) som du kan skicka när du vill.
* När du har valt det här alternativet kommer vi att placera dessa uppgifter i kö i kommandocentralen och liveflödet när du startar Campaign. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i Gmail eller Outlook öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

För efterföljande dagar/steg i din kampanj finns följande alternativ:

Skicka det här e-postmeddelandet samtidigt som det föregående e-postmeddelandet i den här kampanjen

* Det här alternativet skickar e-postmeddelandet samtidigt som e-postmeddelandet direkt före det.
* Det skickas fortfarande den dag det är kopplat till.

Skicka det här e-postmeddelandet vid följande tidpunkt

* När ni får igång er kampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny sändningstid när du stänger av din kampanj.

Skapa en uppgift; Jag skickar det här e-postmeddelandet själv

* Med det här alternativet skapas en e-postaktivitet (och synkroniseras med Salesforce) som du kan skicka när du vill.
* När du har valt det här alternativet kommer Tout att ställa de här uppgifterna i kö när du startar Campaign i kommandocentralen och liveflödet. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i Gmail eller Outlook öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

Koppla det här e-postmeddelandet till föregående e-postmeddelande

* Det här sändningsalternativet är en uppföljning av ditt tidigare e-postmeddelande och kommer att lägga till det föregående e-postmeddelandet längst ned i det här e-postmeddelandet.

>[!MORELIKETHIS]
>
>[Skapa en försäljningskampanj](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target=&quot;_blank&quot;}
>[Stegtyper för säljkampanj och påminnelseaktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target=&quot;_blank&quot;}
>[Inställningar för försäljningskampanj](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target=&quot;_blank&quot;}
