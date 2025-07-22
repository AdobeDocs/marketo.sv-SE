---
unique-page-id: 10096677
description: Testa din ON24-händelseintegrering - Marketo Docs - produktdokumentation
title: Testa din ON24-händelseintegrering
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Testa din ON24-händelseintegrering {#test-your-on-event-integration}

Se till att testa integreringen av dina event noggrant.

## Rekommenderad testsekvens innan din första kampanj körs {#recommended-test-sequence-before-running-your-first-campaign}

1. Fyll i händelsens registreringsformulär och använd en giltig e-postadress för att testa.
1. Bekräfta att testnamnet visas med statusen **Registrerad** i medlemsstödrastret för din Marketo-händelse.
1. Bekräfta att testnamnet också visas som **Registrerad** i ON24.
1. Bekräfta att den giltiga e-postadressen som du använde för att registrera testnamnet fick ett bekräftelsemeddelande via e-post till händelsen och att den unika URL:en matchas i e-postmeddelandet.

   >[!NOTE]
   >
   >Du måste använda token `{{member.webinar url}}` i bekräftelsemeddelandet för att den unika URL:en ska kunna visas i varje registrants e-post.

## Efter händelsen {#after-the-event}

Så här uppdateras data när händelsen har inträffat:

* Marketo hämtar deltagardata från ON24 varje kväll.
* När deltagarens data synkroniseras mellan Marketo och ON24 uppdaterar Marketo medlemskapsstatusen till [!UICONTROL Attended], [!UICONTROL Attended On-demand] eller [!UICONTROL No Show]. Händelsens status uppdateras till **[!UICONTROL Summary]** på fliken **[!UICONTROL Event Complete]**.

>[!MORELIKETHIS]
>
>* [Exempel på ON24-händelseintegrering](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
