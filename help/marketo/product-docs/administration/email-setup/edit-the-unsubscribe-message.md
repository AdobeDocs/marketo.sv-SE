---
unique-page-id: 2360251
description: Redigera avbeställningsmeddelandet - Marketo Docs - Produktdokumentation
title: Redigera avbeställningsmeddelandet
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# Redigera avbeställningsmeddelandet {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

När du skickar e-postmeddelanden om marknadsföring (ej [i drift](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)) läggs text och länkar till längst ned. Du kan ändra standardinställningarna. Så här gör du.

## Redigera avbeställningsmeddelandet {#edit-the-unsubscribe-message-1}

1. Klicka på **E-post** under **Admin**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK##**


1. Redigera **Avbeställ HTML** - och **Avbeställ** text efter behov och klicka på **Spara ändringar**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Där har du den. **Se till att testa!** Du vill inte att dina marknadsföringsmejl ska ha brutna länkar för att avbryta prenumerationen.

>[!TIP]
>
>Du kan anpassa positionen för den HTML-kod som ska avbeställas i ditt e-postmeddelande genom att använda [tokens](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Avbeställ standardtext {#default-unsubscribe-text}

Om du behöver gå tillbaka till systemets standardavbrutna prenumeration kopierar/klistrar du in följande:

Avbeställ HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Avbeställ text:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>* [Redigera meddelandet&quot;Visa som webbsida&quot;](edit-the-view-as-web-page-message.md)

>



