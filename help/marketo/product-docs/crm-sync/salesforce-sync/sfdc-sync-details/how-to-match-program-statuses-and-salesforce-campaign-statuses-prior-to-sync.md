---
unique-page-id: 2360370
description: Matcha programstatus och Salesforce-kampanjstatus före synkronisering - Marketo Docs - produktdokumentation
title: Matcha programstatus och Salesforce-kampanjstatus före synkronisering
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Matcha programstatus och Salesforce-kampanjstatus före synkronisering {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

I den här artikeln beskrivs hur du åtgärdar ett inkompatibelt statusfel och mappar statusvärden innan du synkroniserar Marketo Program och Salesforce Campaign.

## Vad gör du om du fick ett felmeddelande? {#what-do-you-do-if-you-received-an-error-message}

Om du försöker synkronisera till en befintlig Salesforce-kampanj som innehåller leads och kampanjen innehåller en eller flera inkompatibla statusvärden visas ett felmeddelande. Ett Marketo-program och en Salesforce-kampanj *synkroniserar inte* om statusvärdena inte är en exakt matchning.

![](assets/image2015-7-22-9-3a23-3a29.png)

I det här felmeddelandet kan du välja att:

1. Välj en annan kampanj att synkronisera med i listrutan, ELLER
1. Du kan avbryta, åtgärda statusfelen och försöka synkronisera när felen har reparerats. Gör något av följande om du vill åtgärda statusfelen:

   * Logga in i Salesforce och ta bort eller byt namn på de inkompatibla kampanjmedlemsstaterna för att mappa till de Marketo-programstatusar som används för den kanaltyp som är kopplad till ditt Marketo-program.
   * Ändra programstatusvärdena i Marketo för att mappa till de Salesforce Campaign-medlemsstater ni har på plats. Det här är en Marketo Admin-funktion. Mer information finns i [Skapa en programkanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
