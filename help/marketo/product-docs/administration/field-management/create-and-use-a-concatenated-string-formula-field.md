---
unique-page-id: 2360337
description: Skapa och använda ett sammanfogat strängfält (formel) - Marketo Docs - produktdokumentation
title: Skapa och använda ett sammanfogat strängfält (formel)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 1%

---

# Skapa och använda ett sammanfogat strängfält (formel) {#create-and-use-a-concatenated-string-formula-field}

Du kan kombinera värden från flera fält eller skapa ett villkorsvärde med hjälp av ett Marketo Engage-formelfält.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Klicka på **[!UICONTROL New Custom Field]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Välj **[!UICONTROL Formula]** för **[!UICONTROL Type]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Ange en **[!UICONTROL Name]** för fältet och klicka sedan på **[!UICONTROL Create]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Sök efter och markera formelfältet och klicka sedan på **[!UICONTROL Edit Rules]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Lägg till två alternativ och definiera dem som skärmbilden nedan.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Läs mer om [tokens för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Nu kan du lägga till formelfältet som en token i ett e-postmeddelande.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Formelfält kan användas i kolumnerna Landing Pages, emails och Smart List. E-postmeddelanden med formelfält kan _inte_ skickas med en gruppkampanj. Använd en [e-postskripttoken](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) i det här scenariot.

Bra jobbat! Nu har du ett smart fält som vet vilken hälsningsfras som ska inkluderas baserat på kön. Ha så kul och bli kreativ.
