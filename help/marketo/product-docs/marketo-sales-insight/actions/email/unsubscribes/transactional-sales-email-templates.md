---
description: E-postmallar för transaktionsförsäljning - Marketo Docs - Produktdokumentation
title: E-postmallar för transaktionsförsäljning
feature: Sales Insight Actions
exl-id: 0178155e-f01c-449f-b510-40adf718e177
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# E-postmallar för transaktionsförsäljning {#transactional-sales-email-templates}

Om ditt team skickar ut transaktionsbaserade eller icke-kommersiella e-postmeddelanden kan du markera en e-postmall som icke-kommersiell så att den kan kringgå avbeställning.

## Saker att notera {#things-to-note}

* Icke-kommersiella e-postmeddelanden kommer att kringgå avbrutna säljabonnemang och [Marketo Engage-avanmälningskontroll](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, men kommer inte att kringgå [blockerade domäner](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Meddelanden om att avbeställa prenumerationen läggs inte automatiskt till i icke-kommersiella e-postmeddelanden, även om inställningen [append unsubscribe message admin &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} är aktiverad. Det `{{team_unsubscribe}}` [dynamiska fältet](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} kommer dock fortfarande att fylla i teamets meddelande om att avbryta prenumerationen.

## Konfigurera en e-postmall för icke-kommersiell användning {#configure-an-email-template-for-non-commercial-use}

1. Klicka på **Mallar** i sidhuvudet.

   ![](assets/transactional-sales-email-templates-1.png)

1. Sök efter och välj den mall som du vill uppdatera.

   ![](assets/transactional-sales-email-templates-2.png)

1. Aktivera alternativet för icke-kommersiell e-post under Mallinställningar.

   ![](assets/transactional-sales-email-templates-3.png)

## Skicka ett icke-kommersiellt e-postmeddelande {#send-a-non-commercial-email}

>[!NOTE]
>
>När du har valt en person som inte längre prenumererar markeras personen som orange.

1. Klicka på **Disponera** i sidhuvudet. Sök efter och välj önskad icke-kommersiell mall.

   ![](assets/transactional-sales-email-templates-4.png)

1. Användarna ser en banderoll som visar att de har valt en icke-kommersiell e-postmall.

   ![](assets/transactional-sales-email-templates-5.png)

1. Klicka på **Skicka**.

   ![](assets/transactional-sales-email-templates-6.png)

E-postmeddelandet skickas fortfarande även om personen avbeställer prenumerationen.
