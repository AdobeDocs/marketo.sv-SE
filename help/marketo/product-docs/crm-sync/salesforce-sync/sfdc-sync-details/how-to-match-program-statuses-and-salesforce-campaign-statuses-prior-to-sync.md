---
unique-page-id: 2360370
description: Matcha programstatus och Salesforce Campaign-status före synkronisering - Marketo Docs - produktdokumentation
title: Matcha programstatus och Salesforce Campaign-status före synkronisering
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Så här matchar du programstatus och [!DNL Salesforce] kampanjstatus före synkronisering {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

I den här artikeln beskrivs hur du åtgärdar ett inkompatibelt statusfel och mappar statusvärden före synkroniseringen av Marketo-programmet och [!DNL Salesforce] Campaign.

## Vad gör du om du fick ett felmeddelande? {#what-do-you-do-if-you-received-an-error-message}

Om du försöker synkronisera till en befintlig [!DNL Salesforce]-kampanj som innehåller leads och kampanjen innehåller en eller flera inkompatibla statusvärden visas ett felmeddelande. Ett Marketo-program och en [!DNL Salesforce] kampanj *synkroniseras inte* om statusvärdena inte är en exakt matchning.

![](assets/image2015-7-22-9-3a23-3a29.png)

I det här felmeddelandet kan du välja att:

1. Välj en annan kampanj att synkronisera med i listrutan, ELLER
1. Du kan avbryta, åtgärda statusfelen och försöka synkronisera när felen har reparerats. Gör något av följande om du vill åtgärda statusfelen:

   * Logga in på Salesforce och ta bort eller byt namn på de inkompatibla Campaign-medlemsstaterna för att mappa till de Marketo-programstatusar som används för den kanaltyp som är kopplad till ditt Marketo-program.
   * Ändra programstatus i Marketo för att mappa till de Salesforce Campaign-medlemsstater ni har. Det här är en Marketo Admin-funktion. Mer information finns i [Skapa en programkanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.
