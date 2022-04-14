---
description: Förstå alternativ för att skicka säljkampanjer via e-post - Marketo Docs - produktdokumentation
title: Om sändningsalternativ för försäljningskampanj för e-poststeg
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: a0a2c93b89738c048f7aac658be9fa95b5e87f89
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Om sändningsalternativ för försäljningskampanj för e-poststeg {#understanding-sales-campaign-send-options-for-email-steps}

När du skapar en försäljningskampanj har du flera alternativ för hur e-poststegen skapas i Sales Insight-åtgärder. Beroende på var e-postadressen hamnar i er säljkampanj skiljer sig alternativen också åt.

## Skicka-alternativ i första steget {#first-step-send-options}

Om det är ditt första steg och den första dagen i din säljkampanj har du följande alternativ:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

Jag väljer när det här e-postmeddelandet ska skickas

* Med det här alternativet kan du välja&quot;skicka vid&quot;-tid för det första e-postmeddelandet i din säljkampanj när du startar säljkampanjen genom att lägga till personer.

Skicka det här e-postmeddelandet vid följande tidpunkt

* När ni börjar med er säljkampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny&quot;skicka&quot;-tid när du stänger av din säljkampanj.

Skapa en uppgift; Jag skickar det här e-postmeddelandet själv

* Med det här alternativet skapas en e-postaktivitet (och synkroniseras med Salesforce) som du kan skicka när du vill.
* När du har valt detta alternativ kommer vi att placera dessa uppgifter i kö i kommandocentralen och liveflödet när du startar säljkampanjen. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i Gmail eller Outlook öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

## Skicka-alternativ för efterföljande steg {#subsequent-step-send-options}

För efterföljande dagar/steg i din säljkampanj finns följande alternativ:

Skicka det här e-postmeddelandet samtidigt som det föregående e-postmeddelandet i den här försäljningskampanjen

* Det här alternativet skickar e-postmeddelandet samtidigt som e-postmeddelandet direkt före det.
* Det skickas fortfarande den dag det är kopplat till.

Skicka det här e-postmeddelandet vid följande tidpunkt

* När ni börjar med er säljkampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny&quot;skicka&quot;-tid när du stänger av din säljkampanj.

Skapa en uppgift; Jag skickar det här e-postmeddelandet själv

* Med det här alternativet skapas en e-postaktivitet (och synkroniseras med Salesforce) som du kan skicka när du vill.
* När du har valt detta alternativ kommer Säljannonsering att placera dessa uppgifter i kö i kommandocentralen och liveflödet när du startar säljkampanjen. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i Gmail eller Outlook öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

Koppla det här e-postmeddelandet till föregående e-postmeddelande

* Det här sändningsalternativet är en uppföljning av ditt tidigare e-postmeddelande och kommer att lägga till det föregående e-postmeddelandet längst ned i det här e-postmeddelandet.

>[!MORELIKETHIS]
>
>[Skapa en försäljningskampanj](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target=&quot;_blank&quot;}
>[Stegtyper för säljkampanj och påminnelseaktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target=&quot;_blank&quot;}
>[Inställningar för försäljningskampanj](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target=&quot;_blank&quot;}
