---
description: Dynamic Chat - Marketo Docs - produktdokumentation
title: Dynamic Chat verksamhet
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 79b439a9bb3d3cd130eb5a7b52cea13988e7b88e
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Dynamic Chat verksamhet {#dynamic-chat-activities}

Dynamic Chat erbjuder flera filter och utlösare som kan användas i dina smarta listor.

![](assets/dynamic-chat-activities-1.png)

## Definitioner {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>Utlöst</b></td>
    <td>En utlösande händelse inträffar när en besökare uppfyller målinriktningskriterierna för en dialog eller ett konversationsflöde och visas i dialogrutan.
    <br>En utlösande händelse per besökare, per session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Engagerad med ett konversationsflöde/dialog</b></td>
    <td>Ett ärende inträffar första gången en webbbesökare klickar på en fråga i ett Dialog- eller konversationsflöde (klicka på ett flervalsalternativ, skicka information, boka ett möte, öppna ett dokument osv.). Om en besökare öppnar en dialogruta eller ett konversationsflöde, men inte klickar på en uppmaning, är ett engagemang <b>not</b> loggad. 
    <br>En engagemangshändelse per besökare, per session.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Aktiverat med en agent</b></td>
    <td>Händer när en besökare har anslutit till en chattagent.
    <br>En engagerad med agenthändelse per besökare, per session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Interaktion med dokument</b></td>
    <td>Händer när en besökare klickar på ett dokument på ett dokumentkort.
    <br>Det kan finnas flera dokumentinteraktioner per besökare, per session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Uppnådda mål</b></td>
    <td>Händer när en besökare når ett mål. <br>Det kan finnas flera måluppnådda händelser per besökare, per session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Schemalagt möte</b></td>
    <td>Händer när en besökare bokar ett möte med en Dynamic Chat-agent.
    <br>Det kan finnas flera mötesbokade händelser per besökare, per session.</td>
  </tr>
</tbody>
</table>

## Saker att notera {#things-to-note}

* Villkor stöds i flödessteg i Dynamic Chat
* Dynamic Chat-aktiviteter kan synkroniseras till [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* Du kan visa enskilda Dynamic Chat-aktiviteter i aktivitetsloggen för en personpost
