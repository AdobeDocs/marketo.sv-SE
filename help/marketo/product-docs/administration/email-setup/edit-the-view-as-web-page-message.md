---
unique-page-id: 2360253
description: Redigera meddelandet"Visa som webbsida" - Marketo Docs - Produktdokumentation
title: Redigera meddelandet Visa som webbsida
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# Redigera meddelandet Visa som webbsida {#edit-the-view-as-web-page-message}

Så här gör du om du behöver redigera texten [Visa som en webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md).

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Redigera meddelandet Visa som webbsida {#edit-the-view-as-web-page-message-1}

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Den andra delen `##MKT_TOK##` är den personens [!UICONTROL munchkin]-cookie. Den ser till att de kodas korrekt när de klickar på länken.

1. Redigera versionerna **[!UICONTROL View as Web Page HTML]** och **[!UICONTROL View as Web Page Text]** efter dina önskemål och klicka på **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Undvik följande:
>
>* Lägga till ytterligare URL:er i någon av HTML-rutorna
>* Placera HTML i textversionen

Där har du den. Skicka testmejl för att säkerställa formatering.

## Standardtexten &quot;Visa som webbsida&quot; {#default-view-as-web-page-text}

Om du någon gång behöver återställa standardsystemet [!UICONTROL View as Web Page] kopierar/klistrar du in följande:

**[!UICONTROL View as Web Page HTML]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL View as Web Page Text]**:

Om du vill visa det här e-postmeddelandet som en webbsida går du till följande adress:
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`

Så ja!
