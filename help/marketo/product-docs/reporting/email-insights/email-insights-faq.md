---
unique-page-id: 10100257
description: Vanliga frågor om e-postinsikter - Marketo Docs - produktdokumentation
title: Vanliga frågor om e-postinsikter
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Vanliga frågor om e-postinsikter {#email-insights-faq}

## Finns det några skillnader mellan nyckeltal med [!UICONTROL Email Insights] och andra e-postrapporter från Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Ja. [!UICONTROL Email Insights] korrelerar interaktionsmått med deras motsvarande leveransmått för samma e-post som skickas när interaktionsmått beräknas (Öppna frekvens, Klickfrekvens-till-Öppet, Avprenumerationstakt). Om du i [!UICONTROL Email Insights] till exempel tittar på ett tidsseriediagram under den senaste veckan med dagliga neddelningar av Klicka-till-Öppna-hastighet, visar vi nu det verkliga korrelerade förhållandet mellan öppna/klicka/avbryta-prenumerationshändelser baserat på motsvarande leveransmått. Detta är i motsats till beteendet i Intresseutforskaren, som helt enkelt sammanfattar allt. [!UICONTROL Email Insights] ger en mer korrekt bild av engagemangsproportioner.

## Varför stöder [!UICONTROL Email Insights] bara 10 anpassade dimensioner? {#why-does-email-insights-only-support-custom-dimensions}

I många fall räcker det inte med att utöka standardsystemdimensionerna med ytterligare 10 anpassade dimensioner. Det innehåller anpassade dimensioner baserade på segmentering eller programtaggar. I framtiden planerar vi att tillåta kunderna att öka antalet tillåtna anpassade dimensioner.

## Varför kan jag inte återanvända kortplatser för anpassade dimensioner efter att de har tilldelats? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

När en viss anpassad Dimension-plats har tilldelats, kommer mappning av den att orsaka ett fel när tidigare data blandas med en ny innebörd. På grund av detta kan anpassade Dimension-kortplatser inte återanvändas. Detta beteende överensstämmer med andra analysverktyg, som Google Analytics.

## Har [!UICONTROL Email Insights] stöd för e-postmeddelanden från Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Ja. Alla e-postmeddelanden som skickas via Marketo Sales Insights inkluderas i [!UICONTROL Email Insights].

## Stöder [!UICONTROL Email Insights] operativa e-postmeddelanden? {#does-email-insights-support-operational-emails}

Ja. Som standard döljs e-postmeddelanden som används för att visa och fråga. Du kan dock ändra den här inställningen under panelen Personliga inställningar.

## Fångar [!UICONTROL Email Insights] återkommande schemalagda e-postflödessteg eller kör Smart Campaign igen? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Ja och Nej. Med den första versionen av [!UICONTROL Email Insights] hämtas alla e-posthändelser och är tillgängliga för alla återkommande schemalagda eller körda smarta kampanjer igen. Men ni kommer inte att kunna skilja mellan olika delar av den smarta kampanjen. Vi lägger till stöd i nästa version för att hämta information om körningen av Smart Campaign för Open, Click och Unsubscribe för att kunna differentiera.

## Varför visar många mätvärden noll när jag filtrerar efter enhetstyp eller enhets-OS? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Med undantag för Click-to-Open Rate, Open, Clicks och Unsubscribes är alla andra mätvärden som stöds antingen leveranshändelser eller förhållanden som härleds från leveranshändelser. Eftersom enhetstyp och enhets-OS bara gäller för interaktionsmått har vi helt enkelt inte den information som ska visas. Det är till exempel en odefinierad fråga att fråga efter leveransfrekvensen när den filtreras efter Device Type = mobile, eftersom Marketo inte skulle ha fått någon interaktionsstatistik för någon av de underliggande Delivery- och Send-händelserna. Vi utforskar olika sätt att tillämpa enhetstyp och enhets-OS från interaktionsstatistik för förhållanden som omfattar både engagemangs- och leveransstatistik.

## Vad gör [!UICONTROL Email Insights] när vissa e-postklienter blockerar bilder? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Ett vanligt branschproblem är att allt fler e-postklienter stänger av bilder som standard. Inläsning av bilder är grunden för hur Öppna registreras. Det är helt möjligt att en användare kan få ett e-postmeddelande med bilder blockerade, men med texten och länkarna fullt läsbara. Om en användare fick detta och klickade på en länk i det e-postmeddelandet, skulle det resultera i ett scenario för en klickhändelse, men ingen motsvarande Open-händelse för det meddelandet. Marketo e-postinsikter genererar automatiskt alla händelser som saknas. Logiken är identisk med hur Marketo gör detta för e-postprestandarapporten och för e-postanalysområdet i skatteutforskaren.
