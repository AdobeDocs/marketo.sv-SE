---
unique-page-id: 2360337
description: Skapa och använda ett sammanfogat strängfält (formel) - Marketo Docs - produktdokumentation
title: Skapa och använda ett sammanfogat strängfält (formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Skapa och använda ett sammanfogat strängfält (formel) {#create-and-use-a-concatenated-string-formula-field}

Du kan kombinera värden från flera fält eller skapa ett villkorsstyrt värde med hjälp av ett Marketo-formelfält.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Klicka på **[!UICONTROL New Custom Field]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Välj **[!UICONTROL Formula]** för **[!UICONTROL Type]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Ange **[!UICONTROL Name]** för fältet klickar du **[!UICONTROL Create]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Sök och välj formelfält och klicka sedan **[!UICONTROL Edit Rules]**.

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
>Formelfält kan användas på landningssidor, e-postmeddelanden och kolumner för smarta listor (de exporteras inte). E-postmeddelanden med formelfält kan _not_ skickas med en batchkampanj. Använd en [e-postskripttoken](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) i detta scenario.

Bra jobbat! Nu har du ett smart fält som vet vilken hälsningsfras som ska inkluderas baserat på kön. Ha så kul och bli kreativ.
