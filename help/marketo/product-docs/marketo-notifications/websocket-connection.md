---
description: Meddelande - Websocket-anslutning - Marketo Docs - Produktdokumentation
title: Meddelande - Webbsocketanslutning
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Meddelande: Webbsocketanslutning {#notification-websocket-connection}

Det här dokumentet är till för Marketo Engage-användare som har fått följande meddelande i sin Marketo-instans: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Om du eller din organisation använder restriktiva brandväggs- eller proxyserverinställningar kan du eller din nätverksadministratör behöva tillåtslista vissa domäner och IP-adressintervall för att Adobe Marketo Engage ska fungera som förväntat.

Marketo Support har inte konfigurerats för att hjälpa till med implementeringen av nedanstående protokoll. Om du behöver hjälp kan du dela det här dokumentet med IT-avdelningen. Om de begränsar webbåtkomsten via ett tillåtelselista ber du dem lägga till följande domäner (inklusive asterisken) för att tillåta alla Marketo-resurser och webbsocketar:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
