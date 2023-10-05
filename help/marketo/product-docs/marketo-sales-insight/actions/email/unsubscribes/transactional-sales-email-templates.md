---
description: E-postmallar för transaktionsförsäljning - Marketo Docs - Produktdokumentation
title: E-postmallar för transaktionsförsäljning
feature: Sales Insight Actions
exl-id: 0178155e-f01c-449f-b510-40adf718e177
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# E-postmallar för transaktionsförsäljning {#transactional-sales-email-templates}

Om ditt team skickar ut transaktionsbaserade eller icke-kommersiella e-postmeddelanden kan du markera en e-postmall som icke-kommersiell så att den kan kringgå avbeställning.

## Saker att notera {#things-to-note}

* Icke-kommersiella e-postmeddelanden kommer att kringgå avbeställningar av försäljning och [Avbeställ Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Avbeställningsmeddelanden läggs inte automatiskt till icke-kommersiella e-postmeddelanden, även om [append unsubscribe message admin setting](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} kommer fortfarande att fylla i ditt teames meddelande om att avbryta prenumerationen.

## Konfigurera en e-postmall för icke-kommersiell användning {#configure-an-email-template-for-non-commercial-use}

1. Klicka på i sidhuvudet **Mallar**.

   ![](assets/transactional-sales-email-templates-1.png)

1. Sök efter och välj den mall som du vill uppdatera.

   ![](assets/transactional-sales-email-templates-2.png)

1. Aktivera alternativet för icke-kommersiell e-post under Mallinställningar.

   ![](assets/transactional-sales-email-templates-3.png)

## Skicka ett icke-kommersiellt e-postmeddelande {#send-a-non-commercial-email}

>[!NOTE]
>
>När du har valt en person som inte längre prenumererar markeras personen som orange.

1. Klicka på i sidhuvudet **Skapa**. Sök efter och välj önskad icke-kommersiell mall.

   ![](assets/transactional-sales-email-templates-4.png)

1. Användarna ser en banderoll som visar att de har valt en icke-kommersiell e-postmall.

   ![](assets/transactional-sales-email-templates-5.png)

1. Klicka **Skicka**.

   ![](assets/transactional-sales-email-templates-6.png)

E-postmeddelandet skickas fortfarande även om personen avbeställer prenumerationen.
