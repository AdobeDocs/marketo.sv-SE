---
unique-page-id: 2360337
description: Skapa och använda ett sammanfogat strängfält (formel) - Marketo Docs - produktdokumentation
title: Skapa och använda ett sammanfogat strängfält (formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: b13360b009aea869bbd96a9cd0888bb121afdcd2
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Skapa och använda ett sammanfogat strängfält (formel) {#create-and-use-a-concatenated-string-formula-field}

Du kan kombinera värden från flera fält eller skapa ett villkorsstyrt värde med hjälp av ett Marketo-formelfält.

1. Gå till **Administratör** område.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Klicka **Fälthantering**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Klicka **Nytt anpassat fält**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Välj **Formel** för **Typ**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Ange **Namn** för fältet klickar du **Skapa**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Sök och välj formelfält och klicka sedan **Redigera regler**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Lägg till två alternativ och definiera dem som skärmbilden nedan.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Läs mer om [variabler för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Nu kan du lägga till formelfältet som en token i ett e-postmeddelande.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Formelfält kan användas på landningssidor, e-postmeddelanden och kolumner för smarta listor (de exporteras inte). E-postmeddelanden med formelfält kan **not** skickas med en batchkampanj. Använd en [e-postskripttoken](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) i detta scenario.

Bra jobbat! Nu har du ett smart fält som vet vilken hälsningsfras som ska inkluderas baserat på kön. Ha så kul och bli kreativ.
