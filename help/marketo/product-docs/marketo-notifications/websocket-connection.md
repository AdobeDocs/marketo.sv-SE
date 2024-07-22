---
description: Meddelande - Websocket-anslutning - Marketo Docs - Produktdokumentation
title: Meddelande - Webbsocketanslutning
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Meddelande: Webbsocketanslutning {#notification-websocket-connection}

Den här artikeln är avsedd för användare av Marketo Engage som har fått följande meddelande i sin Marketo-instans: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Om du eller din organisation använder restriktiva brandväggs- eller proxyserverinställningar kan du eller din nätverksadministratör behöva tillåtslista vissa domäner och IP-adressintervall för att Adobe Marketo Engage ska fungera som förväntat.

Marketo Support har inte konfigurerats för att hjälpa till med implementeringen av nedanstående protokoll. Om du behöver hjälp kan du dela den här artikeln med IT-avdelningen. Om de begränsar webbåtkomsten via ett tillåtelselista ber du dem lägga till följande domäner (inklusive asterisken) för att tillåta alla Marketo-resurser och webbsocketar:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
