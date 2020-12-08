---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Product Documentation
title: Push to Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Push to Sales Connect {#push-to-sales-connect}

Knappen Push to Tout (Skicka till toning) innehåller en lista över dina leads/kontakter i Salesforce och placerar dem i en grupp i Sales Connect. Du kan sedan snabbt skicka en anpassningsbar gruppe-post med Tout-spårning bifogad.

## Krav {#requirements}

* Sales Connect [Salesforce-paket](http://docs.marketo.com/x/C4PS) installerat av `Salesforce Admin`

* `Push to Sales Connect`knapp installerad för att visa en lista per `Salesforce Admin`

* Salesforce-anslutning skapad med Sales Connect för användare som gör push

## Använda {#how-to}

1. Klicka på fliken **Lead/kontakt** i Salesforce.
1. Växla till listvyn som du vill skicka till Sales Connect bredvid knappen Gå.
1. Klicka på **Gå**.
1. Markera alla leads/kontakter som du vill ska pushas för att tona ut.
1. Välj **Push to MSE**.
1. Ett nytt fönster visas som verifierar antalet leads/kontakter som du vill skicka över. Välj **Gå till grupp**. Sales Connect `will not push over` för alla kontakter som är markerade som `Email Opt Out` i Salesforce eller `Unsubscribed` i Sales Connect.

   >[!NOTE]
   >
   >Sales Connect kommer att lägga till den här gruppen med namnet &quot;SFDC-..&quot; till sidan Relationer i [webbprogrammet](http://toutapp.com/login).

1. Välj **E-posta hela gruppen** om du vill skicka det här gruppe-postmeddelandet.

