---
unique-page-id: 14352621
description: Understanding Send Options - Marketo Docs - Product Documentation
title: Förstå sändningsalternativ
exl-id: acdee691-478e-4ffe-90e2-54cf559fa38d
feature: Marketo Sales Connect
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Förstå sändningsalternativ {#understanding-send-options}

När du skapar en kampanj har du flera alternativ för hur e-poststegen skapas i [!DNL Sales Connect]. Och beroende på var e-postmeddelandet hamnar i din kampanj skiljer sig även alternativen åt.

Om det är ditt första steg och den första dagen i din kampanj har du följande alternativ:

![](assets/image2019-10-25-10-43-19.png)

**Jag väljer när det här e-postmeddelandet ska skickas**

* Med det här alternativet kan du välja&quot;skicka vid&quot;-tid för det första e-postmeddelandet i din kampanj när du startar kampanjen genom att lägga till personer.

**Skicka det här e-postmeddelandet vid följande tidpunkt**

* När ni får igång er kampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny sändningstid när du stänger av din kampanj.

**Skapa en aktivitet. Jag skickar det här e-postmeddelandet själv**

* Det här alternativet skapar en [!UICONTROL Email Task] (och synkroniserar till [!DNL Salesforce]) som du kan skicka när du vill.
* När du har valt det här alternativet kommer vi att placera dessa uppgifter i kö i kommandocentralen och liveflödet när du startar Campaign. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i [!DNL Gmail] eller [!DNL Outlook] öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

För efterföljande dagar/steg i din kampanj finns följande alternativ:

**Skicka det här e-postmeddelandet samtidigt som det föregående e-postmeddelandet i kampanjen**

* Det här alternativet skickar e-postmeddelandet samtidigt som e-postmeddelandet direkt före det.
* Det skickas fortfarande den dag det är kopplat till.

>[!IMPORTANT]
>
>Det går inte att skicka e-postmeddelanden samtidigt som föregående e-postmeddelande för e-postmeddelanden som skickas samma dag. I stället skickas e-postmeddelandet när det e-postmeddelande som skickats från föregående dag skickas. Om det här alternativet väljs för ett e-postmeddelande den första dagen i kampanjen (rekommenderas inte) skickas det e-postmeddelandet direkt i början av kampanjen.

**Skicka det här e-postmeddelandet vid följande tidpunkt**

* När ni får igång er kampanj genom att lägga till personer i den kommer vi att schemalägga e-postmeddelandet för den här gången.
* Du har alltid möjlighet att välja en ny sändningstid när du stänger av din kampanj.

**Skapa en aktivitet. Jag skickar det här e-postmeddelandet själv**

* Det här alternativet skapar en [!UICONTROL Email Task] (och synkroniserar till [!DNL Salesforce]) som du kan skicka när du vill.
* När du har valt det här alternativet kommer Tout att ställa de här uppgifterna i kö när du startar Campaign i kommandocentralen och liveflödet. Du kan sedan anpassa och skicka (eller schemalägga) varje e-postmeddelande innan det skickas ut.

   * Om du öppnar den här uppgiften i webbprogrammet öppnas ett dispositionsfönster med kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer.
   * Om du öppnar den här uppgiften i [!DNL Gmail] eller [!DNL Outlook] öppnas ett fönster för inbyggda dispositioner där kontaktens e-postadress, ämnesraden i ditt e-postmeddelande och den mall du väljer fylls i dynamiskt.

**Koppla det här e-postmeddelandet till föregående e-postmeddelande**

* Det här sändningsalternativet är en uppföljning av ditt tidigare e-postmeddelande och kommer att lägga till det föregående e-postmeddelandet längst ned i det här e-postmeddelandet.
