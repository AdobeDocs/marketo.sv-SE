---
unique-page-id: 2360337
description: Skapa och använda ett sammanfogat strängfält (formel) - Marketo Docs - Produktdokumentation
title: Skapa och använda ett sammanfogat strängfält (formel)
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# Skapa och använd ett sammanfogat strängfält (formel) {#create-and-use-a-concatenated-string-formula-field}

Du kan kombinera värden från flera fält eller skapa ett villkorsstyrt värde med hjälp av ett Marketo-formelfält.

1. Gå till **Admin** och klicka på **Fälthantering**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Klicka på **Nytt anpassat fält**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Välj **Formel** som **Typ**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Ange ett **namn** för fältet och klicka sedan på **Skapa**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Sök efter och markera formelfältet och klicka sedan på **Redigera regler**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Lägg till två alternativ och definiera dem som skärmbilden nedan.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   Läs mer om [token för flödessteg](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Nu kan du lägga till formelfältet som en token i ett e-postmeddelande.

   ![](assets/seven.png)

Bra jobbat! Nu har du ett smart fält som vet vilken hälsningsfras som ska inkluderas baserat på kön. Ha så kul och bli kreativ.

>[!NOTE]
>
>Formelfält kan användas på landningssidor, i e-postmeddelanden och i kolumner för smarta listor. de inte exporteras. E-postmeddelanden med formelfält kan inte skickas via batchkampanjer

