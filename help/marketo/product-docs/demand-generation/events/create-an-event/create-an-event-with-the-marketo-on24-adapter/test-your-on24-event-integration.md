---
unique-page-id: 10096677
description: Testa din ON24-händelseintegrering - Marketo Docs - produktdokumentation
title: Testa din ON24-händelseintegrering
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Testa din ON24-händelseintegrering {#test-your-on-event-integration}

Se till att testa integreringen av dina event noggrant.

## Rekommenderad testsekvens innan din första kampanj körs {#recommended-test-sequence-before-running-your-first-campaign}

1. Fyll i händelsens registreringsformulär och använd en giltig e-postadress för att testa.
1. Bekräfta att testnamnet visas med en **Registrerad** i medlemsrutnätet för din Marketo-händelse.
1. Bekräfta att testnamnet också visas som **Registrerad** i ON24.
1. Bekräfta att den giltiga e-postadressen som du använde för att registrera testnamnet fick ett bekräftelsemeddelande via e-post till händelsen och att den unika URL:en matchas i e-postmeddelandet.

   >[!NOTE]
   >
   >Du måste använda `{{member.webinar url}}` token i bekräftelsemeddelandet för att den unika URL:en ska visas i varje registrants e-postadress.

## Efter händelsen {#after-the-event}

Så här uppdateras data när händelsen har inträffat:

* Marketo hämtar deltagardata från ON24 varje kväll.
* När deltagarens data synkroniseras mellan Marketo och ON24 uppdaterar Marketo medlemskapsstatusen till Bifogad, Vid behov eller Ingen visning. I händelsens **Sammanfattning** -fliken uppdateras händelsens status till **Händelsen har slutförts**.

>[!MORELIKETHIS]
>
>* [Exempel på händelseintegrering ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
>* [Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}

