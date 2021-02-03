---
unique-page-id: 10096683
description: ON24 Event Registration Updates - Marketo Docs - produktdokumentation
title: ON24 - Händelseregistreringsuppdateringar
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# ON24-händelseregistreringsuppdateringar {#on-event-registration-updates}

## Manuellt godkända registranter {#manually-approving-registrants}

Du kan godkänna dina registranter manuellt innan du skickar en bekräftelse via e-post. Om du vill göra det måste du konfigurera kampanjerna så att de hanterar det här steget till:

1. För kampanjen Registreringsutlösare:

   * I den smarta listan ställer du in utlösaren på **Fyller i formulär**.
   * I Flow ställer du in Status in Progression till **Pending Approval**.

1. Gå till Händelse och klicka på fliken **Medlemmar**. På den här fliken visas alla personer som har fyllt i formuläret. Deras status ska vara **Väntande godkännande**.
1. Använd filtret längst upp i rutnätet om du bara vill visa personer med statusen **Väntande godkännande**.
1. Markera de personer som du vill registrera (Skift-klicka, Ctrl-klicka eller Markera alla).
1. Klicka på **Ändra status** på menyn. Välj **Registrerad**, **Avvisad** eller någon annan tillämplig status.

## Hantera personer med ett registreringsfel {#handling-people-with-a-registration-error}

Om en person slutar att registreras utan att anges till statusfelet Registreringsfel är det inte för sent att återskapa.

1. Filtrera listan med personer med statusen **Registreringsfel** på fliken Medlemmar.
1. Innan du fortsätter bör du kontrollera att du har fastställt och åtgärdat problemet med integreringen (kontrollera att det inte finns några fel under **Event Partners** i Admin).
1. När problemet är löst markerar du alla personer med registreringsfelstatus och ändrar deras status till **Registrerad**. Detta kommer att försöka registrera dem igen med ON24.

## Uppdaterar medlemsstatus från ON24 {#updating-member-status-from-on}

Marketo hämtar automatiskt information om närvaro vid ungefär 200 Pacific varje kväll. Om du vill uppdatera närvaroinformationen manuellt klickar du på **Uppdatera från webbinariet Provider** under **Händelseåtgärder**.

>[!MORELIKETHIS]
>
>[Om Marketo ON24-adapterhändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
