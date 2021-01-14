---
unique-page-id: 2360251
description: Redigera avbeställningsmeddelandet - Marketo Docs - Produktdokumentation
title: Redigera avbeställningsmeddelandet
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# Redigera avbeställningsmeddelandet {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

När du skickar marknadsföringsmeddelanden (icke-[operativ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)) läggs text och länkar för att avbryta prenumerationen till längst ned. Du kan ändra standardinställningarna. Så här gör du.

## Redigera avbeställningsmeddelandet {#edit-the-unsubscribe-message-1}

1. Under **Admin** klickar du på **E-post**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >* **%mkt_opt_out_prefix%**
   >* **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK##**


1. Redigera versionerna **Avbeställ HTML** och **Avbeställ Text** om du vill och klicka på **Spara ändringar**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Där har du den. _Se till att testa!_ Du vill inte att dina marknadsföringsmejl ska ha brutna länkar för att avbryta prenumerationen.

>[!TIP]
>
>Du kan anpassa positionen för HTML-avanmälan i ditt e-postmeddelande genom att använda [tokens](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Standardtext för att avbryta prenumeration {#default-unsubscribe-text}

Om du behöver gå tillbaka till systemets standardavbrutna prenumeration kopierar/klistrar du in följande:

Avbeställ HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Avbeställ text:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Redigera meddelandet&quot;Visa som webbsida&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
