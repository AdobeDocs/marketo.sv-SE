---
unique-page-id: 10096683
description: ON24 Event Registration Updates - Marketo Docs - Product Documentation
title: ON24 - Händelseregistreringsuppdateringar
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# ON24 - Händelseregistreringsuppdateringar {#on-event-registration-updates}

>[!IMPORTANT]
>
>Från och med augusti 2022 har ON24 inte längre stöd för nya Marketo-integreringar. Informationen i den här artikeln gäller endast befintliga användare.

## Manuellt godkända registranter {#manually-approving-registrants}

Du kan godkänna dina registranter manuellt innan du skickar en bekräftelse via e-post. Om du vill göra det måste du konfigurera kampanjerna så att de hanterar det här steget till:

1. För kampanjen Registreringsutlösare:

   * Ställ in utlösaren på **Fyller i formulär**.
   * I Flödet anger du status i progression till **Väntar på godkännande**.

1. Gå till händelsen och klicka på knappen **Medlemmar** -fliken. På den här fliken visas alla personer som har fyllt i formuläret. Deras status bör vara inställd på **Väntar på godkännande**.
1. Använd filtret längst upp i rutnätet för att endast visa personer med statusen **Väntar på godkännande**.
1. Markera de personer som du vill registrera (Skift-klicka, Ctrl-klicka eller Markera alla).
1. Klicka på **Ändra status**. Välj **Registrerad**, **Avvisad** eller någon annan tillämplig status.

## Hantera personer med ett registreringsfel {#handling-people-with-a-registration-error}

Om en person slutar att registreras utan att anges till statusfelet Registreringsfel är det inte för sent att återskapa.

1. Filtrera listan med personer med statusen på fliken Medlemmar **Registreringsfel**.
1. Kontrollera att du har fastställt och åtgärdat problemet med integreringen innan du fortsätter (kontrollera att det inte finns några fel under **Event Partners** i Admin).
1. När problemet är löst väljer du alla personer med status Registreringsfel och ändrar deras status till **Registrerad**. Detta kommer att försöka registrera dem igen med ON24.

## Uppdaterar medlemsstatus från ON24 {#updating-member-status-from-on}

Marketo hämtar automatiskt information om närvaro vid ungefär 200 PST varje kväll. Om du vill uppdatera närvaroinformation manuellt klickar du på **Uppdatera från webbseminarieleverantör** under **Händelseåtgärder**.

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
