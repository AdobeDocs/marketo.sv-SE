---
unique-page-id: 2360253
description: Redigera meddelandet"Visa som webbsida" - Marketo Docs - Produktdokumentation
title: Redigera meddelandet"Visa som webbsida"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Redigera meddelandet&quot;Visa som webbsida&quot; {#edit-the-view-as-web-page-message}

Om du behöver redigera[Visa som en webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;text, så här.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Redigera meddelandet&quot;Visa som webbsida&quot; {#edit-the-view-as-web-page-message-1}

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Den andra delen `##MKT_TOK##` är [!UICONTROL munchkin] den personens kaka. Den ser till att de kodas korrekt när de klickar på länken.

1. Redigera **[!UICONTROL View as Web Page HTML]** och **[!UICONTROL View as Web Page Text]** versioner som du vill ha och klicka på **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Undvik följande:
>
>* Lägga till ytterligare URL:er i någon av rutorna HTML
>* Placera HTML i textversionen


Där har du den. Skicka testmejl för att säkerställa formatering.

## Standardtexten &quot;Visa som webbsida&quot; {#default-view-as-web-page-text}

Om du någon gång behöver återgå till standardsystemet[!UICONTROL View as Web Page]&quot;, kopiera/klistra in följande:

**[!UICONTROL View as Web Page HTML]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL View as Web Page Text]**:

Om du vill visa det här e-postmeddelandet som en webbsida går du till följande adress:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Så ja!
