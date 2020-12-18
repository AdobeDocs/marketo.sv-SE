---
unique-page-id: 2949158
description: Integrera RTP med Google Analytics - Marketo Docs - Produktdokumentation
title: Integrera RTP med Google Analytics
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---


# Integrera RTP med Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics är nu en driftstandard och alla egenskaper i Google har uppgraderats till Universal Analytics.
>
>I den här artikeln beskrivs hur du använder den gamla Google Standard Analytics, men vi rekommenderar att du går över till Universal Analytics.
>
>Om du inte redan använder [analytics.js-spårningskoden](https://developers.google.com/analytics/devguides/collection/analyticsjs/) rekommenderar Google att du taggar om webbplatsen så att den används. Följande har tagits bort av Google:
>
>* ga.js
>* urchin.js
>* WAP-/serversidesfragment
>* JT / MO
>* Egna variabler
>* Användardefinierade variabler

>
>
Se hur du kan integrera [webbpersonalisering med Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

## Introduktion {#introduction}

Analysera webbanalysen från en ny vinkel med hjälp av direkt dataflöde från Marketo Real-Time Personalization (RTP) till Google Analytics (GA). Mät era webbbesök i GA enligt organisationer, branscher och RTP-kampanjer. Se mätvärden som olika branscher eller RTP-segment i GA och hur de fungerar och genererar leads utifrån olika trafikkällor (sociala, betalda, organiska), analysera klickfrekvenser på kampanjer och mäta vilken effekt personaliseringskampanjer har på er webbplats. Utnyttja den här möjligheten för att få ut maximalt av ditt RTP-konto

**RTP Audience Analytics**

Med integreringen får du en ny dimension på ditt GA-konto. RTP förbättrar automatiskt dina instrumentpaneler med:

1. Organisationer och branscher
1. Anpassade segment i RTP
1. Kontobaserade marknadsföringslistor

Fokusera på B2B-utsikterna. Analysera kanalerna utifrån riktade branscher och segment.

## Kanalrapport {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2B Dashboard hjälper er att förstå hur besökarna delas upp efter vertikala värden och RTP-segmentering. Ni kan se hur besökarna presterar i enlighet med finansbranschen och olika marknadsföringskampanjer (betalda, organiska, sociala). Kontrollpanelen ger även en översikt på hög nivå över hur dina RTP-segment fungerar och visar hur de största organisationerna besöker webbplatsen.

## Beteendeflöde {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

I beteendeflödesrapporten (se bild) visas den sökväg som besökare reser från en sida eller händelse till nästa. Bilden visar vägen för alla besökare från finanssektorn. Den här rapporten kan hjälpa er att identifiera vilket innehåll som håller besökarna engagerade med er webbplats.

## RTP-prestanda {#rtp-performance}

Mät era RTP-kampanjer och korrelera dem med det övergripande genomsnittliga antalet webbplatser. Lär dig hur de här kampanjerna påverkar era webbplatsmätningar och använd dessa data för att fokusera era personaliseringssatsningar på rätt mål. Generera anpassade rapporter för att bättre förstå hur era personaliseringskampanjer fungerar.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Konfigurera RTP med Google Analytics {#setting-up-rtp-with-google-analytics}

1. Lägg till e-postadressen [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#0674727628616734466b67746d6372692865696b) som en Läs och analysera-användare till ditt GA-konto. Mer information finns i [här](https://support.google.com/analytics/answer/2884495?hl=en).
1. I ditt RTP-konto. Gå till **Kontoinställningar**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Under **Kontoinställningar**, **Domän** och **Analytics**
1. Klicka på** Google Analytics.**
1. Aktivera relevanta **anpassade variabler** och **händelser** för att lägga till data från RTP till Google Analytics.
1. Ange **kortplatsen** för att skicka anpassade variabeldata (standard är 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

Klicka på **SPARA**.

>[!NOTE]
>
>För att kunna skicka segmentdata till GA markerar du kryssrutan **Skicka händelse till Google Analytics på segmentmatchning** under sidan [Redigera segment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) på RTP-plattformen.

## Konfigurera Google Analytics-rapporter med RTP-data {#setting-up-google-analytics-reports-with-rtp-data}

I Google Analytics kan du använda kontrollpaneler, GA-segmentering och rapportering för att visa dina RTP-data:

* [På ](https://support.google.com/analytics/answer/1068216?hl=en) kontrollpanelerna finns en översikt över webbplatsens prestanda.
* Ett GA-segment är avsett att filtrera besökare i GA-gränssnittet och visa trafiken per segment. Se hur du skapar ett segment [här](https://support.google.com/analytics/answer/3124493?hl=en).
* Skapar [anpassade rapporter](https://support.google.com/analytics/answer/1033013?hl=en) för att visa och/eller konfigurera schemalagda e-postmeddelanden. Se under Anpassning > Ny anpassad rapport.
