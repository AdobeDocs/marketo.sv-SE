---
unique-page-id: 10096683
description: ON24 Event Registration Updates - Marketo Docs - Product Documentation
title: ON24 - Händelseregistreringsuppdateringar
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# ON24 - Händelseregistreringsuppdateringar {#on-event-registration-updates}

## Manuellt godkända registranter {#manually-approving-registrants}

Du kan godkänna dina registranter manuellt innan du skickar en bekräftelse via e-post. Om du vill göra det måste du konfigurera kampanjerna så att de hanterar det här steget till:

1. För kampanjen Registreringsutlösare:

   * I [!UICONTROL Smart List] ställer du in utlösaren på **[!UICONTROL Fills Out Form]**.
   * Ange [!UICONTROL Status in Progression] som **[!UICONTROL Pending Approval]** i flödet.

1. Gå till Händelsen och klicka på fliken **[!UICONTROL Members]**. På den här fliken visas alla personer som har fyllt i formuläret. Deras status bör anges till **[!UICONTROL Pending Approval]**.
1. Använd filtret längst upp i rutnätet om du bara vill visa personer med statusen **[!UICONTROL Pending Approval]**.
1. Markera de personer som du vill registrera (Skift-klicka, Ctrl-klicka eller Markera alla).
1. Klicka på **[!UICONTROL Change Status]** på menyn. Välj **[!UICONTROL Registered]**, **[!UICONTROL Rejected]** eller någon annan tillämplig status.

## Hantera personer med ett registreringsfel {#handling-people-with-a-registration-error}

Om en person inte registreras utan anges till statusen [!UICONTROL Registration Error] är det inte för sent att återskapa.

1. Filtrera listan med personer med statusen [!UICONTROL Members] på fliken **[!UICONTROL Registration Error]**.
1. Innan du fortsätter bör du kontrollera att du har fastställt och åtgärdat problemet med integrering (kontrollera att det inte finns några fel under **[!UICONTROL Event Partners]** i Admin).
1. När problemet är löst markerar du alla personer med statusen [!UICONTROL Registration Error] och ändrar deras status till **[!UICONTROL Registered]**. Detta kommer att försöka registrera dem igen med ON24.

## Uppdaterar medlemsstatus från ON24 {#updating-member-status-from-on}

Marketo hämtar automatiskt information om närvaro vid ungefär 200 PST varje kväll. Om du vill uppdatera närvaroinformation manuellt klickar du på **[!UICONTROL Refresh from Webinar Provider]** under **[!UICONTROL Event Actions]**.

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
