---
unique-page-id: 2949160
description: Integrera med Adobe Analytics - Marketo Docs - produktdokumentation
title: Integrera med Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Integrera med Adobe Analytics {#integrate-with-adobe-analytics}

## Intro {#intro}

Analysera webbanalysen utifrån B2B-perspektiv genom att visa kampanjdata för organisation, bransch och Marketo Real-Time Personalization (RTP) i ditt Adobe Analytics-konto.

Det här dokumentet möjliggör integrering mellan Marketo Real-Time Personalization (RTP) och Adobe Adobe Analytics. Med hjälp av data från RTP kan ni identifiera och analysera trender i alla branschsegment och organisationer som besöker er webbplats och mäta effektiviteten i era RTP-kampanjer, och få insikter och analyser för att få optimala resultat.

Ni kan uppnå detta genom att titta på mätvärden som antalet nya jämfört med återkommande besökare i varje segment, analysera klickfrekvenser på kampanjer och identifiera vilka branscher och anpassade segment och realtidskampanjer som genererade de bästa konverteringsleads. Utnyttja den här möjligheten för att få ut maximalt av ditt RTP-konto.

## RTP Audience Analytics {#rtp-audience-analytics}

Med RTP - AA-integrering får du en ny dimension i webbanalysgränssnittet. RTP förbättrar automatiskt instrumentpanelerna för webbanalys med:

1. Organisations- och branschdata
1. Anpassade RTP-segment
1. Listor med namngivna konton (Account-Based Marketing)

Detta förbättrar era B2B-data och gör att ni kan fokusera på relevanta besökare genom att optimera:

1. Utgående kanaler
1. Innehåll
1. Återmarknadsföring

## Kanalrapport {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP-instrumentpanelen hjälper dig att förstå hur besökarna delas upp efter vertikala linjer och RTP-segment. Ni kan se hur besökarna presterar utifrån branschen och olika marknadsföringskampanjer (betalda, organiska, sociala) som är relaterade till den branschen. Kontrollpanelen ger också en översikt på hög nivå över vilka avsnitt besökarna visar beroende på vilken typ av bransch de använder.

## Beteenderapport {#behavioral-report}

Olika beteenderapporter kan skapas i Adobe Analytics utifrån data om organisation, bransch och RTP-segment. Dessa flödesrapporter visualiserar den sökväg besökarna tar från en sida eller händelse till nästa. Den här rapporten kan hjälpa er att identifiera vilket innehåll som håller besökarna engagerade med er webbplats.

## RTP-prestanda {#rtp-performance}

Visa visningar och konverteringar för RTP-kampanjer under Anpassade länkar i Adobe Analytics.

Denna Custom Link-rapport visar visningar och konverteringar av kampanjer i följande namnformat:

* Impression ISegment: [RTP-segmentnamn], ICampaign: [Namn på RTP-kampanj]
* Konvertering av ISegment: [RTP-segmentnamn], ICampaign: [Namn på RTP-kampanj]

![](assets/custom-links-report.png)

## Konfigurera i Adobe Analytics {#set-up-in-adobe-analytics}

Integreringen använder det JavaScript-API som finns i Adobe Analytics. Anpassade konverteringsvariabler (eVar), anpassade händelser (händelse) och trafikvariabler används i integreringen. Alla måste aktiveras inifrån en AA-administratör. Du måste ange konverteringsvariabler, anpassade händelser och trafikvariabler i annars kan du inte se data i sviten även om du aktiverat den i RTP.

Gör så här för att konfigurera dessa variabler i AA:

1. Gå till **Administratörsverktyg** på ditt AA-konto.
1. Välj **Report Suite** som ska användas med integreringen.
1. Under **Redigera inställningar**, gå till **Konvertering** och markera **[Konverteringsvariabler](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Välj [Konverteringsvariabel](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) nummer (vi rekommenderar):

   1. Evar # 20 for Industry Custom Conversions
   1. Evar # 21 for Organization Custom Conversions

   >[!NOTE]
   >
   >Välj ett annat tillgängligt nummer om du väljer #. Justera det här numret mot platsnumret i RTP-kontoinställningarna.

   1. Ändra status till _Aktiverad_.

      1. Ändra namn till **Bransch** och **Organisation**. (Så här kommer det att se ut i Report Suite.)

      1. Ändra fältet Förfaller efter till **Besök**.


1. Under **Redigera inställningar** gå till **Konvertering** och markera **[Success Events](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Välj ett anpassat händelsenummer för lyckade händelser (vi rekommenderar):

      1. event20 för RTP-kampanjer
      1. event21 för RTP-segment

      >[!NOTE]
      >
      >Välj ett annat tillgängligt nummer om du väljer #. Justera det här numret mot platsnumret i RTP-kontoinställningarna.

      1. Ändra namnen på de två händelserna till **RTP-kampanjer** och **RTP-segment**. Det här namnet visas i rapportsviten.
   1. Markera textfältet som ska **Räknare (inga underrelationer)**



1. Under **Redigera inställningar** gå till **[Trafik](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** och markera **[Trafikvariabler](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Välj egenskapsnumret för trafikvariabeln (vi rekommenderar):

      1. Egenskap nr 20 - Namn: RTP-segmentorganisation
      1. Egenskap nr 21 - Namn: RTP-segmentindustri
      1. Egenskap nr 25 - Namn: Kampanjorganisation
      1. Egenskap nr 26 - Namn: RTP Campaign Industry

      >[!NOTE]
      >
      >Välj ett annat tillgängligt nummer om du väljer #. Justera det här numret mot platsnumret i RTP-kontoinställningarna)

      1. Ändra egenskapsnamnen för 4. Det här namnet visas i rapportsviten.
   1. Välj aktiverat fält att **Aktiverad**.

   1. Markera fältet Sökvägsrapporter till **Aktiverad**.



## Konfigurera i Marketo Real-Time Personalization (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. På RTP-plattformen går du till **Kontoinställningar**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Under **Kontoinställningar**, klicka **Domän**.
1. Under **Analyser, klicka** **Adobe Analytics**.
1. Sväng **På** variabeln Conversion, Custom och Traffic växlar.
1. Tilldela konverterings-, händelse- och trafikvariabler **platsnummer** för att matcha platsnumren som skapats i AA
1. Klicka **Spara**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Våra rekommenderade inställningar för kortplatser är
>
>**Konverteringsvariabler**
>
>* Anpassade branschkonverteringar - fack 20
>* Anpassade organisationskonverteringar - plats 21
>
>**Anpassade händelser**
>
>* Anpassad kampanjhändelse - kortplats 20
>* Anpassad händelse för segment - plats 21
>
>**Trafikvariabler**
>
>* Segmentorganisationstrafikvariabel - fack 20
>* Segmentbranschens trafikvariabel - fack 21
>* Trafikvariabel för kampanjorganisation - kortplats 22
>* Trafikvariabel för kampanjbransch - kortplats 23
>
>**Se till att platsnumren är justerade mot de variabler och händelsenummer som skapas i AA.**

## Rapporter {#reports}

Skapa förbättrade SiteAdobe Analytics-rapporter utifrån organisationsnamn, branscher och RTP-segment samt kampanjdata i realtid.

Exempel på anpassade rapporter och kontrollpaneler i AA är:

* Prestanda efter bransch eller definierat segment (kontobaserade namngivna listor)
* Branschanalys per nyckeltal
* Visa sidor per organisation
* Marknadsföringskanalernas prestanda enligt Organisation, Bransch, Segment

**-Report Examples-**

**Top Industries Report**

![](assets/top-industries-report.png)

**Organisationsrapport**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Skapa RTP-instrumentpanelen**

Skapa en [ny instrumentpanel](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), anropas **Kontrollpanel för RTP**. Den här instrumentpanelen hjälper dig att förstå hur besökarna delas upp efter vertikala linjer och RTP-segment.

1. Klicka **Instrumentpanel,** klicka **Lägg till instrumentpanel**.

1. Namnge instrumentpanelen **Kontrollpanel för RTP**.

1. Välj **storlek för instrumentpanel** 3 x 2, 2 x 2.

1. Skapa [reportlet](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) och lägga till [innehåll på kontrollpanelen](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Lägga till branschrapporten på kontrollpanelen

1. Gå till **Anpassade konverteringar**, klicka på **Bransch**.

1. Konfigurera diagram till **Cirkeldiagram**.

1. Klicka på **Kontrollpanel**, lägga till **Portlet**.

1. Namnge rapporten **Top Industries**.

1. Placera på kontrollpanelen **Kontrollpanel för RTP**.

1. Skapa **Nytt**.

Lägga till segmentrapporten på kontrollpanelen

1. Gå till **Webbplatsmått**. Klicka på **Anpassade händelser**, **Segment**.

1. Konfigurera diagram till **Lodrätt streck**.

1. Klicka på **Kontrollpanel**, lägga till **Portlet**.

1. Namnge rapporten **Övre segment**.

1. Placera på kontrollpanelen **Kontrollpanel för RTP**.

1. Skapa **Nytt**.

Dina rapporter visas på kontrollpanelen.

## Visa bilder och klick (konverteringar) i Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Klicka **Anpassade länkar**.

   ![](assets/sitecatalyst1-1.png)

1. Sök efter Impressions för att visa segmenterings- och kampanjnamn som representerar antalet visningar för kampanjen.\
   ![](assets/sitecatalyst1.png)

1. Sök efter konvertering om du vill visa segment- och kampanjnamn som representerar antalet klick för kampanjen.

   ![](assets/sitecatalyst2.png)
