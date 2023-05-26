---
description: Förstå alternativ för att skicka säljkampanjer via e-post - Marketo Docs - produktdokumentation
title: Om sändningsalternativ för försäljningskampanj för e-poststeg
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 1934cbd4a941fdfc1110c6934da66e58042aa572
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Om sändningsalternativ för försäljningskampanj för e-poststeg {#understanding-sales-campaign-send-options-for-email-steps}

När du skapar en försäljningskampanj har du flera alternativ för hur e-poststegen skapas i Sales Insight-åtgärder. Beroende på var e-postadressen hamnar i er säljkampanj skiljer sig alternativen också åt.

## Skicka-alternativ i första steget {#first-step-send-options}

Om det är ditt första steg och den första dagen i din säljkampanj har du följande alternativ:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Jag väljer när det här e-postmeddelandet ska skickas {#first-step-i-will-choose}

* Med det här alternativet kan du välja&quot;skicka vid&quot;-tid för det första e-postmeddelandet i din säljkampanj när du startar säljkampanjen genom att lägga till personer.

### Skicka det här e-postmeddelandet vid följande tidpunkt {#first-step-following-time}

* När ni börjar med er säljkampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny&quot;skicka&quot;-tid när du stänger av din säljkampanj.

### Skapa en uppgift; Jag skickar det här e-postmeddelandet själv {#first-step-create-a-task}

* Med det här alternativet skapas en e-postaktivitet (och synkroniseras med Salesforce) som du kan skicka när du vill.
* När du har valt detta alternativ kommer vi att placera dessa uppgifter i kö i kommandocentralen och liveflödet när du startar säljkampanjen. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i Gmail eller Outlook öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

## Skicka-alternativ för efterföljande steg {#subsequent-step-send-options}

För efterföljande dagar/steg i din säljkampanj finns följande alternativ:

### Skicka det här e-postmeddelandet samtidigt som det föregående e-postmeddelandet i den här försäljningskampanjen {#subsequent-send-at-same-time}

* Det här alternativet skickar e-postmeddelandet samtidigt som e-postmeddelandet direkt före det.
* Det skickas fortfarande den dag det är kopplat till.

### Skicka det här e-postmeddelandet vid följande tidpunkt {#subsequent-send-at-following-time}

* När ni börjar med er säljkampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny&quot;skicka&quot;-tid när du stänger av din säljkampanj.

### Skapa en uppgift; Jag skickar det här e-postmeddelandet själv {#subsequent-create-a-task}

* Med det här alternativet skapas en e-postaktivitet (och synkroniseras med Salesforce) som du kan skicka när du vill.
* När du har valt detta alternativ kommer Säljannonsering att placera dessa uppgifter i kö i kommandocentralen och liveflödet när du startar säljkampanjen. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i Gmail eller Outlook öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

### Skapa det här e-postmeddelandet som en uppföljning av föregående e-postmeddelande i kampanjen {#subsequent-create-this-email}

* Aktivera den här kryssrutan om du vill att det föregående e-postmeddelandet i din säljkampanj ska bifogas till nästa e-postmeddelande som din försäljningskampanj skickar ut.
* För den bifogade kopian av e-postmeddelandet skickas alltid e-postmallen i din försäljningskampanj ut. Ändringar som användaren har gjort innan det skickades kommer inte att tas med i sändningen.

>[!NOTE]
>
>Det här alternativet för att skapa ett e-postmeddelande som uppföljning är endast tillgängligt i ett e-poststeg när det föregående steget också är ett e-postmeddelande. Om föregående steg är Anropa, InMail eller Egen visas inte alternativet att skapa en uppföljning.

>[!MORELIKETHIS]
>
>[Skapa en försäljningskampanj](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>[Stegtyper för säljkampanj och påminnelseaktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>[Inställningar för försäljningskampanj](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}
