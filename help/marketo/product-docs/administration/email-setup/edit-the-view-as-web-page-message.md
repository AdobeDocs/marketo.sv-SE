---
unique-page-id: 2360253
description: Redigera meddelandet"Visa som webbsida" - Marketo Docs - Produktdokumentation
title: Redigera meddelandet"Visa som webbsida"
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Redigera meddelandet &quot;Visa som webbsida&quot; {#edit-the-view-as-web-page-message}

Så här redigerar du texten [Visa som en webbsida](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md).

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Redigera meddelandet &quot;Visa som webbsida&quot; {#edit-the-view-as-web-page-message-1}

1. Under **Admin** klickar du på **E-post**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Följande variabler är viktiga. Ta inte bort dem!
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK#
   >    
   >    
   >Den andra delen ##MKT_TOK## är den personens munchkincookie. Den ser till att de kodas korrekt när de klickar på länken.

1. Redigera **Visa som webbsida HTML** och **Visa som webbsidetext **versioner efter dina önskemål och klicka på **Spara ändringar**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Undvik följande:
>
>* Lägga till ytterligare URL:er i någon av HTML-rutorna
>* Placera HTML i textversionen

>



Där har du den. Skicka testmejl för att säkerställa formatering.

## Standardtexten &quot;Visa som webbsida&quot; {#default-view-as-web-page-text}

Om du vill återgå till standardsystemet &quot;Visa som webbsida&quot; kopierar/klistrar du in följande:

**Visa som webbsidesHTML:**
`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **Visa som webbsidetext:**

Om du vill visa det här e-postmeddelandet som en webbsida går du till följande adress:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom! Du är klar.
