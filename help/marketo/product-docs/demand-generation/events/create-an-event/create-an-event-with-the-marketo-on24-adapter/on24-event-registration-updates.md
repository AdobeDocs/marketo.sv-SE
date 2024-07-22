---
unique-page-id: 10096683
description: ON24 Event Registration Updates - Marketo Docs - Product Documentation
title: ON24 - Händelseregistreringsuppdateringar
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# ON24 - Händelseregistreringsuppdateringar {#on-event-registration-updates}

## Manuellt godkända registranter {#manually-approving-registrants}

Du kan godkänna dina registranter manuellt innan du skickar en bekräftelse via e-post. Om du vill göra det måste du konfigurera kampanjerna så att de hanterar det här steget till:

1. För kampanjen Registreringsutlösare:

   * I den smarta listan ställer du in utlösaren på **Fyller i formulär**.
   * I Flödet anger du statusen i progression till **Väntar på godkännande**.

1. Gå till händelsen och klicka på fliken **Medlemmar**. På den här fliken visas alla personer som har fyllt i formuläret. Deras status ska vara **Väntande godkännande**.
1. Använd filtret längst upp i rutnätet om du bara vill visa personer med statusen **Väntar på godkännande**.
1. Markera de personer som du vill registrera (Skift-klicka, Ctrl-klicka eller Markera alla).
1. Klicka på **Ändra status** på menyn. Välj **Registrerad**, **Avvisad** eller någon annan tillämplig status.

## Hantera personer med ett registreringsfel {#handling-people-with-a-registration-error}

Om en person slutar att registreras utan att anges till statusfelet Registreringsfel är det inte för sent att återskapa.

1. Filtrera listan med personer med statusen **Registreringsfel** på fliken Medlemmar.
1. Innan du fortsätter bör du kontrollera att du har fastställt och åtgärdat problemet med integrering (kontrollera att det inte finns några fel under **Event Partners** i Admin).
1. När problemet är löst väljer du alla personer med status Registreringsfel och ändrar deras status till **Registrerad**. Detta kommer att försöka registrera dem igen med ON24.

## Uppdaterar medlemsstatus från ON24 {#updating-member-status-from-on}

Marketo hämtar automatiskt information om närvaro vid ungefär 200 PST varje kväll. Om du vill uppdatera närvaroinformationen manuellt klickar du på **Uppdatera från webbinariet-providern** under **Händelseåtgärder**.

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
