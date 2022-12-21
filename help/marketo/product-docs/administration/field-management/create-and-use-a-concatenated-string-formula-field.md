---
unique-page-id: 2360337
description: Skapa och använda ett sammanfogat strängfält (formel) - Marketo Docs - produktdokumentation
title: Skapa och använda ett sammanfogat strängfält (formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Skapa och använda ett sammanfogat strängfält (formel) {#create-and-use-a-concatenated-string-formula-field}

Du kan kombinera värden från flera fält eller skapa ett villkorsstyrt värde med hjälp av ett Marketo-formelfält.

1. Gå till **Administratör** och klicka **Fälthantering**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Klicka **Nytt anpassat fält**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Välj **Formel** för **Typ**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Ange **Namn** för fältet klickar du **Skapa**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Sök och välj formelfält och klicka sedan **Redigera regler**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Lägg till två alternativ och definiera dem som skärmbilden nedan.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Läs mer om [variabler för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Nu kan du lägga till formelfältet som en token i ett e-postmeddelande.

   ![](assets/seven.png)

>[!NOTE]
>
>Formelfält kan användas på landningssidor, e-postmeddelanden och kolumner för smarta listor (de exporteras inte). E-postmeddelanden med formelfält kan **not** skickas med en batchkampanj. Använd en [e-postskripttoken](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) i detta scenario.

Bra jobbat! Nu har du ett smart fält som vet vilken hälsningsfras som ska inkluderas baserat på kön. Ha så kul och bli kreativ.
