---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Product Documentation
title: Push to Sales Connect
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Skicka till Sales Connect {#push-to-sales-connect}

Knappen Push to Tout (Skicka till toning) innehåller en lista över dina leads/kontakter i Salesforce och placerar dem i en grupp i Sales Connect. Du kan sedan snabbt skicka en anpassningsbar gruppe-post med Tout-spårning bifogad.

## Krav {#requirements}

* Sales Connect Salesforce-paket installerat av Salesforce Admin

* Knappen Skicka till försäljningskontakt installerad i listvyn av Salesforce Admin

* Salesforce-anslutning skapad med Sales Connect för användare som gör push

## Så här {#how-to}

1. Klicka på fliken **Lead/kontakt** i Salesforce.
1. Växla till listvyn som du vill skicka till Sales Connect bredvid knappen Gå.
1. Klicka på **Gå**.
1. Markera alla leads/kontakter som du vill ska pushas för att tona ut.
1. Välj **Skicka till MSE**.
1. Ett nytt fönster visas som verifierar antalet leads/kontakter som du vill skicka över. Välj **Gå till grupp**. Sales Connect kommer inte att föra över kontakter som är markerade som e-postavanmälan i Salesforce eller Avanmäl i Sales Connect.

   >[!NOTE]
   >
   >Sales Connect kommer att lägga till den här gruppen med namnet &quot;SFDC-..&quot; till sidan Relationer på [webbprogrammet](http://toutapp.com/login).

1. Välj **E-posta hela gruppen** om du vill skicka ut gruppe-postmeddelandet.
