---
description: Konfiguration - Marketo Docs - produktdokumentation
title: Konfiguration
feature: Dynamic Chat
exl-id: 01ca6a38-4918-46b0-b0f6-1baffbb0bbaf
source-git-commit: 42e2a23c1c451c61fd62237fd1305924b51437b2
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Konfiguration {#configuration}

Lär dig hur du anpassar utseendet på chatbot-dialogrutan.

Kom igång genom att klicka på **Chatbot** under **Konfiguration**.

![](assets/configuration-1.png)

Det finns flera olika anpassningsalternativ.

![](assets/configuration-2.png)

## Fliken Format {#style-tab}

### Stil {#style}

Här definierar du utseendet och känslan för den chattbot där dina dialogrutor ska visas, inklusive: färger, teckensnitt, placering av robotwidgeten och chatbogens namn/avatar.

Färgen för varje kategori bestäms av ett [hexadecimalt färgvärde](https://color.adobe.com/create/color-wheel){target="_blank"} (t.ex. vitt = #ffffff, rött = #bf1932, osv.).

![](assets/configuration-3.png)

Med ankarpunkten kan besökaren öppna/stänga chatbox. Du kan välja om ikonen ska visas längst ned till höger eller längst ned till vänster. Du kan också öka/minska utfyllnaden (mängden utrymme mellan ikonen och webbsidans nederkant).

![](assets/configuration-4.png)

### Punktinställningar {#agent-settings}

I Bot Settings kan du lägga till en etikett i din chatbox (t.ex. &quot;Adobe Assistant&quot;) som visas högst upp i den. Du kan också fastställa fördröjningen för svar (i sekunder) och ändra din chattavatar. Klicka på knappen **+** om du vill överföra din egen avatarbild.

![](assets/configuration-5.png)

>[!NOTE]
>
>Anpassade avatarer ska vara fyrkantiga bilder som är mindre än 256 kb och mindre än 200 x 200 px. Filtyper som stöds: .jpg, .png, .gif, .webp, .svg.

**Nytt meddelandeljud**

Klicka på listrutan för att välja ett ljud för besökaren varje gång som chattbot aktiveras i en session. Det finns flera ljud att välja mellan.

**Aktivera penselmeddelanden på mobilen**

Välj reglaget för att aktivera&quot;Poke&quot;, som visar den inledande frågan bredvid chattikonen utan att besökaren behöver klicka på den för att se den, för besökare som chattar in från en mobil enhet.

![](assets/configuration-6.png)

>[!NOTE]
>
>Poke är bara tillgängligt på det första [kortet](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"} i konversationen.

Kom ihåg att klicka på **Spara** när du är klar med ändringarna.

![](assets/configuration-7.png)

## Sekretessflik {#privacy-tab}

Klicka på fliken **Sekretess** för att lägga till/redigera URL:en för webbplatsens sekretesspolicy (valfritt).

![](assets/configuration-8.png)

## Installationsflik {#installation-tab}

För att chattbot ska visas på webbplatsen måste du först installera Dynamic Chat JavaScript-fragmentet. Klicka på den här fliken om du vill söka efter/kopiera den nödvändiga koden. Om du inte känner till den här åtgärden kan du kontakta ditt webbteam eller din IT-avdelning för att få hjälp.

![](assets/configuration-9.png)

>[!TIP]
>
>Titta efter vad som ska läggas till om webbplatsen använder CSP (Content-Security-Policy) nedan.

>[!NOTE]
>
>Marketo Support har inte konfigurerats för att hjälpa till med felsökning av HTML. Kontakta en webbutvecklare om du behöver hjälp med HTML.
