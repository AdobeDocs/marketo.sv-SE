---
unique-page-id: 2360251
description: Redigera avbeställningsmeddelandet - Marketo Docs - produktdokumentation
title: Redigera avbeställningsmeddelandet
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---

# Redigera avbeställningsmeddelandet {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

När du skickar e-postmarknadsföring (icke-[operativ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)) läggs text och länkar till längst ned. Du kan ändra standardinställningarna. Så här gör du.

## Var ska du göra redigeringen? {#where-to-make-the-edit}

1. Gå till **[!UICONTROL Admin]** -avsnitt.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. Redigera **[!UICONTROL Unsubscribe HTML]** och **[!UICONTROL Unsubscribe Text]** versioner som du vill ha och klicka på **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Där har du den. _Se till att testa!_ Du vill inte att dina marknadsföringsmejl ska ha brutna länkar för att avbryta prenumerationen.

>[!TIP]
>
>Du kan anpassa HTML för att avsluta prenumerationen i ditt e-postmeddelande genom att använda [variabler](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Avbeställ standardtext {#default-unsubscribe-text}

Om du behöver gå tillbaka till systemets standardavbrutna prenumeration kopierar/klistrar du in följande:

[!UICONTROL Unsubscribe HTML]:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` [!UICONTROL Unsubscribe Text]:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Redigera meddelandet&quot;Visa som webbsida&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
