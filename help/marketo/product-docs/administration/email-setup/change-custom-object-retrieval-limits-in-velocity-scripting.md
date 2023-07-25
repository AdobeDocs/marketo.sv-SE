---
description: "Ändra hämtningsgränser för anpassade objekt i [!DNL Velocity Scripting] - Marketo Docs - produktdokumentation"
title: "Ändra hämtningsgränser för anpassade objekt i [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# Ändra hämtningsgränser för anpassade objekt i [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Om du använder [!DNL Velocity Script] den här funktionen kan vara till för dig om du vill visa anpassade objektdata i e-postmeddelanden. Som standard har du åtkomst till 10 överordnade anpassade objekt från Snabbredigeringsskript. Om du behöver få tillgång till mer kan du läsa vidare.

## Vad är [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) är ett språk som bygger på [!DNL Java] som utformats för att malla och skripta HTML-innehåll. Marketo tillåter att den används i e-postsammanhang genom [skripttoken](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Detta ger bland annat åtkomst till data som lagras i anpassade objekt.

Du kan referera till överordnade och underordnade anpassade objekt som är direkt kopplade till lead- eller kontaktpersonen, men inte till anpassade objekt på tredje nivån. För varje anpassat objekt är de 10 senast uppdaterade posterna per person/kontakt tillgängliga vid körning och beställs från den senast uppdaterade (vid 0) till den äldsta (vid 9).

## Ändra gränsen {#how-to-change-the-limit}

1. Gå till **[!UICONTROL Admin]** -avsnitt.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. I [!UICONTROL Custom Object Retrieval Limits] tabell, ange en ny [!UICONTROL Parent Retrieval Limit] och klicka **[!UICONTROL Save Changes]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>The [!UICONTROL Parent Retrieval Limit] värdet måste vara mellan 10 och 100. The [!UICONTROL Child Retrieval Limit] ställs in automatiskt åt dig. Detta görs genom att dividera 1000 med [!UICONTROL Parent Retrieval Limit]. Om du t.ex. anger gränsen för Överordnad till 50 blir gränsen för Underordnad 20 (1 000‡ 50 = 20).

Snyggt! Nu kan du få åtkomst till fler anpassade objekt från [!DNL Velocity script].
