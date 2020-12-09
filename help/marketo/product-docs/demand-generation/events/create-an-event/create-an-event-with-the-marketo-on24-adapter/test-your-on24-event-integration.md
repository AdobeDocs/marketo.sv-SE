---
unique-page-id: 10096677
description: Testa din ON24-händelseintegrering - Marketo Docs - produktdokumentation
title: Testa din ON24-händelseintegrering
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Testa din ON24-händelseintegrering {#test-your-on-event-integration}

Se till att testa integreringen av dina event noggrant.

## Rekommenderad testsekvens innan din första kampanj körs {#recommended-test-sequence-before-running-your-first-campaign}

1. Fyll i händelsens registreringsformulär och använd en giltig e-postadress för att testa.
1. Bekräfta att testnamnet visas med **statusen Registrerad** i medlemskapsmätaren för Marketo-händelsen.
1. Bekräfta att testnamnet också visas som **Registrerat** i ON24.
1. Bekräfta att den giltiga e-postadressen som du använde för att registrera testnamnet fick ett bekräftelsemeddelande via e-post till händelsen och att den unika URL:en matchas i e-postmeddelandet.

   >[!NOTE]
   >
   >Du måste använda token i ditt bekräftelsemeddelande för att den unika URL:en ska kunna visas i varje registrants e-postmeddelande. `{{member.webinar url}}`

## Efter händelsen {#after-the-event}

Så här uppdateras data när händelsen har inträffat:

* Marketo hämtar deltagardata från ON24 varje kväll.
* När deltagarens data synkroniseras mellan Marketo och ON24 uppdaterar Marketo medlemskapsstatusen till Bifogad, Vid behov eller Ingen visning. På fliken **Sammanfattning** för händelsen uppdateras händelsens status till **Händelse klar**.

>[!MORELIKETHIS]
>
>* [Exempel på händelseintegrering ON24](example-on24-event-integration.md)
>* [Om Marketo ON24-adapterhändelser](understanding-marketo-on24-adapter-events.md)

>



