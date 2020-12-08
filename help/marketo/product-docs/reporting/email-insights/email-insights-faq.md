---
unique-page-id: 10100257
description: E-postinsikter - frågor och svar - Marketo Docs - Produktdokumentation
title: Vanliga frågor om e-postinsikter
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Vanliga frågor om e-postinsikter {#email-insights-faq}

## Finns det några skillnader mellan nyckeltal med e-postinsikter och andra marknads-e-postrapporter? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Ja. E-postinsikter korrelerar interaktionsstatistik med deras motsvarande leveransmått för samma e-post som skickas när interaktionsstatistik beräknas (Öppna frekvens, Klickfrekvens-till-Öppet, Avbeställningsfrekvens). I e-postinsikter, till exempel, när vi tittar på ett tidsseriediagram över den senaste veckan med dagliga uppdelningar av Klicka-till-öppna-hastighet, visar vi nu det verkliga korrelerade förhållandet mellan öppna/klicka/avprenumerera-händelser baserat på motsvarande leveransmått. Detta är i motsats till beteendet i Intresseutforskaren, som helt enkelt sammanfattar allt. Insikter om e-post ger en mer korrekt bild av engagemangsgraden.

## Varför stöder e-postinsikter endast 10 anpassade Dimensioner? {#why-does-email-insights-only-support-custom-dimensions}

I många fall räcker det inte med att utöka standardsystemdimensionerna med ytterligare 10 anpassade dimensioner. Det innehåller anpassade dimensioner baserade på segmentering eller programtaggar. I framtiden planerar vi att tillåta kunderna att öka antalet tillåtna anpassade Dimensioner.

## Varför kan jag inte återanvända anpassade Dimensioner när de har tilldelats? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

När en viss anpassad Dimension har tilldelats, kommer mappning att göra att tidigare data genererar ett fel när de blandas med en ny innebörd. På grund av detta kan det hända att anpassade Dimensioner inte återanvänds. Detta beteende överensstämmer med andra mätverktyg, som Google Analytics.

## Har e-postinsikter stöd för Marketo Sales Insight-e-postmeddelanden? {#does-email-insights-support-marketo-sales-insight-emails}

Ja. Alla e-postmeddelanden som skickas via Marketo Sales Insights ingår i E-postinsikter.

## Har e-postinsikter stöd för operativ e-post? {#does-email-insights-support-operational-emails}

Ja. Som standard döljs e-postmeddelanden som används för att visa och fråga. Du kan dock ändra den här inställningen under panelen Personliga inställningar.

## Fångar e-postinsikter återkommande schemalagda eller kör Smart Campaign-e-postflödet igen? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Ja och Nej. I den första versionen av e-postinsikter hämtas alla e-posthändelser och är tillgängliga för alla återkommande schemalagda eller omkörda Smart Campaign. Men ni kommer inte att kunna skilja mellan olika delar av den smarta kampanjen. Vi lägger till stöd i nästa version för att hämta information om körningen av Smart Campaign för Open, Click och Unsubscribe för att kunna differentiera.

## Varför visar många mätvärden noll när jag filtrerar efter enhetstyp eller enhets-OS? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Med undantag för Click-to-Open Rate, Open, Clicks och Unsubscribes är alla andra mätvärden som stöds antingen leveranshändelser eller förhållanden som härleds från leveranshändelser. Eftersom enhetstyp och enhets-OS bara gäller för interaktionsmått har vi helt enkelt inte den information som ska visas. Det är till exempel en odefinierad fråga att fråga efter leveransfrekvensen när den filtreras efter Device Type = mobile, eftersom Marketo inte skulle ha fått någon interaktionsstatistik för någon av de underliggande Delivery- och Send-händelserna. Vi utforskar olika sätt att tillämpa enhetstyp och enhets-OS från interaktionsstatistik för förhållanden som omfattar både engagemangs- och leveransstatistik.

## Vad gör e-postinsikter när vissa e-postklienter blockerar bilder? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Ett vanligt branschproblem är att allt fler e-postklienter stänger av bilder som standard. Inläsning av bilder är grunden för hur Öppna registreras. Det är helt möjligt att en användare kan få ett e-postmeddelande med bilder blockerade, men med texten och länkarna fullt läsbara. Om en användare fick detta och klickade på en länk i det e-postmeddelandet, skulle det resultera i ett scenario för en klickhändelse, men ingen motsvarande Open-händelse för det meddelandet. Marketo Email Insights genererar automatiskt alla händelser som saknas. Logiken är identisk med hur Marketo gör detta för e-postrapporten och för e-postanalysdelen i skatteutforskaren.
