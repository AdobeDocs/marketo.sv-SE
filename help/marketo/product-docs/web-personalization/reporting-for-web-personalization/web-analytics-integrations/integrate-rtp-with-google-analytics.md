---
unique-page-id: 2949158
description: Integrera RTP med Google Analytics - Marketo Docs - produktdokumentation
title: Integrera RTP med Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Integrera RTP med Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics är nu den operativa standarden och alla egenskaper i Google har uppgraderats till Universal Analytics.
>
>I den här artikeln beskrivs hur du använder den gamla Google Standard Analytics, men vi rekommenderar att du går över till Universal Analytics.
>
>Om du inte redan använder [analytics.js tracking code](https://developers.google.com/analytics/devguides/collection/analyticsjs/)rekommenderar Google att du taggar om webbplatsen för att använda den. Följande har tagits bort av Google:
>
>* ga.js
>* urchin.js
>* WAP-/serversidesfragment
>* JT / MO
>* Egna variabler
>* Användardefinierade variabler
>
>Se hur ni kan integrera [Webbpersonalisering med Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introduktion {#introduction}

Analysera webbanalysen från en ny vinkel med hjälp av direkt dataflöde från Marketo Real-Time Personalization (RTP) till Google Analytics (GA). Mät era webbbesök i GA enligt organisationer, branscher och RTP-kampanjer. Se mätvärden som olika branscher eller RTP-segment i GA och hur de fungerar och genererar leads utifrån olika trafikkällor (sociala, betalda, organiska), analysera klickfrekvenser på kampanjer och mäta vilken effekt personaliseringskampanjer har på er webbplats. Utnyttja den här möjligheten för att få ut maximalt av ditt RTP-konto

**RTP Audience Analytics**

Med integreringen får du en ny dimension på ditt GA-konto. RTP förbättrar automatiskt dina instrumentpaneler med:

1. Organisationer och branscher
1. Anpassade segment i RTP
1. Account-Based Marketing

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

1. Lägg till e-postadressen rtp.ga2@gmail.com som en Läs och analysera-användare på ditt GA-konto. Mer information finns i [här](https://support.google.com/analytics/answer/2884495?hl=en).

1. I ditt RTP-konto. Gå till **Kontoinställningar**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Under **Kontoinställningar**, **Domän** och **Analyser**.

1. Klicka på **Google Analytics**.

1. Aktivera relevant **Anpassade variabler** och **Händelser** att lägga till dessa data från RTP till Google Analytics.

1. Ange **Plats** talet för att skicka anpassade variabeldata (standard är 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Klicka **Spara**.

>[!NOTE]
>
>För att kunna skicka segmentdata till GA, under [Redigera segmentsida](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) Markera kryssrutan i RTP-plattformen **Skicka händelse till Google Analytics på segmentmatchning**.

## Konfigurera Google Analytics-rapporter med RTP-data {#setting-up-google-analytics-reports-with-rtp-data}

I Google Analytics kan du använda kontrollpaneler, GA-segmentering och rapportering för att visa dina RTP-data:

* [Kontrollpaneler](https://support.google.com/analytics/answer/1068216?hl=en) ger en översikt över webbplatsens prestanda.
* Ett GA-segment är avsett att filtrera besökare i GA-gränssnittet och visa trafiken per segment. Se hur du skapar ett segment [här](https://support.google.com/analytics/answer/3124493?hl=en).
* Skapar [skräddarsydda rapporter](https://support.google.com/analytics/answer/1033013?hl=en) för att visa och/eller konfigurera schemalagda e-postmeddelanden. Se under Anpassning > Ny anpassad rapport.
