---
unique-page-id: 10096677
description: Testa din ON24-händelseintegrering - Marketo Docs - produktdokumentation
title: Testa din ON24-händelseintegrering
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Testa din ON24-händelseintegrering {#test-your-on-event-integration}

>[!IMPORTANT]
>
>Från och med augusti 2022 har ON24 inte längre stöd för nya Marketo-integreringar. Informationen i den här artikeln gäller endast befintliga användare.

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
>* [Exempel på händelseintegrering ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

