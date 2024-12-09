---
unique-page-id: 2360251
description: Redigera avbeställningsmeddelandet - Marketo Docs - produktdokumentation
title: Redigera avbeställningsmeddelandet
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---

# Redigera avbeställningsmeddelandet {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

När du skickar marknadsföringsmeddelanden (icke-[operativ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)) läggs text och länkar för att avbryta prenumerationen till längst ned. Du kan ändra standardinställningarna. Så här gör du.

## Var ska du göra redigeringen? {#where-to-make-the-edit}

1. Gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Redigera versionerna **[!UICONTROL Unsubscribe HTML]** och **[!UICONTROL Unsubscribe Text]** efter dina önskemål och klicka på **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Där har du den. _Se till att testa!_ Du vill inte att dina marknadsföringsmeddelanden ska innehålla brutna länkar för att avbryta prenumerationen.

>[!TIP]
>
>Du kan anpassa positionen för det avbrutna HTML i ditt e-postmeddelande genom att använda [tokens](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Avbeställ standardtext {#default-unsubscribe-text}

Om du behöver gå tillbaka till systemets standardavbrutna prenumeration kopierar/klistrar du in följande:

[!UICONTROL Unsubscribe HTML]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Unsubscribe Text]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Redigera meddelandet Visa som webbsida](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
