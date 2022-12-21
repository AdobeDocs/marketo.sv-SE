---
unique-page-id: 14352477
description: Skicka till Sales Connect - Marketo Docs - produktdokumentation
title: Push to Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Push to Sales Connect {#push-to-sales-connect}

Knappen Push to Tout (Skicka till toning) innehåller en lista över dina leads/kontakter i Salesforce och placerar dem i en grupp i Sales Connect. Du kan sedan snabbt skicka en anpassningsbar gruppe-post med Tout-spårning bifogad.

## Krav {#requirements}

* Sales Connect Salesforce-paket installerat av Salesforce Admin

* Knappen Skicka till försäljningskontakt installerad i listvyn av Salesforce Admin

* Salesforce-anslutning skapad med Sales Connect för användare som gör push

## Använda {#how-to}

1. Klicka på **Lead/kontakt** i Salesforce.
1. Växla till listvyn som du vill skicka till Sales Connect bredvid knappen Gå.
1. Klicka **Gå**.
1. Markera alla leads/kontakter som du vill ska pushas för att tona ut.
1. Välj **Skjut till MSE**.
1. Ett nytt fönster visas som verifierar antalet leads/kontakter som du vill skicka över. Välj **Gå till grupp**. Sales Connect kommer inte att föra över kontakter som är markerade som e-postavanmälan i Salesforce eller Avanmäl i Sales Connect.

   >[!NOTE]
   >
   >Sales Connect kommer att lägga till den här gruppen med namnet &quot;SFDC-..&quot; till sidan Relationer på sidan [webbprogram](https://toutapp.com/login).

1. Välj **E-posta hela gruppen** för att skicka ut det här gruppmeddelandet.
