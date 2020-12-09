---
unique-page-id: 2951884
description: Understanding Opportunity Analysis in Revenue Explorer - Marketo Docs - produktdokumentation
title: Förstå säljprojektsanalys i skatteutforskaren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---


# Förstå säljprojektsanalys i skatteutforskaren {#understanding-opportunity-analysis-in-revenue-explorer}

Med säljprojektsanalys i intäktsutforskaren kan du undersöka dina möjligheter på en djupare nivå. Segmentera och dela upp data baserat på eventuella lead-/företagsattribut, t.ex. lead source, industry eller geography. Analysera skapandet av affärsmöjligheten och stäng utifrån namn, fas eller sannolikhet. Ta reda på marknadsbidragen till pipeline.

## Exempelanalys {#example-analysis}

Här är några rapporter som du kan skapa i området för säljprojektsanalys.

1. Marknadsföringspåverkan på skapade affärsmöjligheter

   Hur stor procentandel av företagets pipeline påverkades av era marknadsföringsprogram? Den här rapporten ger dig svaret. I följande cirkeldiagram visas hur stor procentandel av antalet affärsmöjligheter och det antal affärsmöjligheter som förvärvats av ett marknadsföringsprogram.

   ![](assets/image2015-7-21-16-3a21-3a4.png)

1. Marknadsföringspåverkan på stängda och vunna affärsmöjligheter
1. Rapporten visar hur mycket intäkter som har förvärvats och påverkats av marknadsföringen, per antal och belopp.

   ![](assets/image2015-7-21-16-3a41-3a55.png)

1. Affärsmöjligheten stängd av lead-källa
1. Den här rapporten redogör för alla möjligheter som stängts av lead-källan och ger en tydlig översikt över vilka källor som fungerar och vilka som inte gör det.

   ![](assets/image2015-7-21-10-3a34-3a50.png)

1. Tid att stänga efter källa

   Den här rapporten visar förhållandet mellan de genomsnittliga dagarna för stängning av en affärsmöjlighet och lead-källan.

   ![](assets/image2015-7-21-10-3a35-3a3.png)

1. Öppen möjlighet och fas

   Den här rapporten visar hur många möjligheter som är öppna i varje skede av intäktscykeln.

   ![](assets/image2015-7-21-10-3a35-3a32.png)

1. Antal affärsmöjligheter per år efter bransch

   Den här rapporten besvarar frågan:&quot;Får vi fler eller färre möjligheter från vissa branscher år för år?&quot;

   ![](assets/image2015-7-21-10-3a35-3a45.png)

## Dimensioner och åtgärder för analys av affärsmöjligheter {#opportunity-analysis-dimensions-and-measures}

Med säljprojektsanalys får du tillgång till alla lead-, företags- och affärsmöjlighetsrelaterade dimensioner och affärsmöjlighetsrelaterade mått. Använd de här dimensionerna för affärsmöjlighetsanalys och åtgärderna för att besvara specifika frågor i rapporten.

1. Företagsattribut

   | Dimension | Beskrivning |
   |---|---|
   | Årsintäkt | Företagets årsomsättning |
   | Ort | Ort där företaget är beläget |
   | Land | Land där företaget är beläget |
   | Bransch | Branschen som företaget är i |
   | Företag | Företagets namn |
   | Antal anställda | Antal anställda i företaget |
   | Postnummer | Företagets postnummer |
   | SIC-kod | Företagets SIC-kod |
   | Läge | Delstaten där företaget är beläget |

1. Leadattribut

   | Dimension | Beskrivning |
   |---|---|
   | Blocklist | Lead är blocklist |
   | Konverterad till affärsmöjlighet | Lead konverteras till en affärsmöjlighet |
   | Ogiltig e-postadress | Om leadet har en giltig e-postadress |
   | Marknadsföring har pausats | Är ledtråden inaktiverad från marknadsföringsmeddelanden? |
   | E-postadress | Leads e-postadress |
   | Befattning | Leads befattning |
   | Fullständigt namn | Lead&#39;s full name |
   | Ursprunglig källtyp | Leads ursprungliga källtyp |
   | Registerkälltyp | Leads registrerade källtyp |
   | Leadägarens e-postadress | Leadägarens e-postadress |
   | Lead Owner Job Title | Leadägarens befattning |
   | Leadägarens namn | Leadägarens namn |
   | Leadkälla | Leadkälla |
   | Leadstatus | Leadstatus |

1. Lead skapad tidsram

   | Dimension | Beskrivning |
   |---|---|
   | Lead skapad i år | Det år då leadet skapades |
   | Lead skapad i kvartal | Kvartalet när leadet skapas |
   | Månad för lead skapad | Den månad då leadet skapas |
   | Lead skapad vecka | Veckan då leadet skapas |
   | Lead skapad den | Det datum då leadet skapades |

1. Attribut för affärsmöjlighet

   | Dimension | Beskrivning |
   |---|---|
   | Affärsmöjligheten har stängts | Är affärsmöjligheten stängd |
   | Prognoskategori för affärsmöjlighet | Prognoskategori för affärsmöjlighet |
   | Affärsmöjlighetens namn | Affärsmöjlighetens namn |
   | Affärsmöjlighet | Möjlighetsfas |
   | Typ av affärsmöjlighet | Typ av affärsmöjlighet |
   | Vunnen affärsmöjlighet | Är den här affärsmöjligheten stängd och vunnen |
   | Marknadsföringspåverkad affärsmöjlighet | Den här flaggan anger om någon av ledtrådarna/kontakterna har förvärvats eller uppnåtts i något marknadsföringsprogram. Endast program som har en periodkostnad definierad beaktas. |

1. Tidsram för stängd affärsmöjlighet

   | Dimension | Beskrivning |
   |---|---|
   | Affärsmöjligheten stängd år | Det år då affärsmöjligheten stängs |
   | Stängt säljprojekt kvartal | Kvartalet när affärsmöjligheten stängs |
   | Stängd månad för affärsmöjlighet | Den månad då affärsmöjligheten stängs |
   | Stängd vecka för affärsmöjlighet | Veckan då affärsmöjligheten stängs |
   | Stängningsdatum för affärsmöjlighet | Datumet då affärsmöjligheten stängs |

1. Tidsram skapad för affärsmöjlighet

   | Dimension | Beskrivning |
   |---|---|
   | Skapad affärsmöjlighet år | Det år då affärsmöjligheten skapas |
   | Möjligheter skapad i kvartal | Kvartalet när affärsmöjligheten skapas |
   | Skapad månad för affärsmöjlighet | Den månad då affärsmöjligheten skapades |
   | Vecka för skapad affärsmöjlighet | Veckan då affärsmöjligheten skapas |
   | Skapad affärsmöjlighet | Datumet då affärsmöjligheten skapas |

1. Åtgärder

   | Mät | Beskrivning |
   |---|---|
   | Genomsnittligt antal dagar för stängning av affärsmöjlighet | Genomsnittligt antal dagar för att stänga en affärsmöjlighet |
   | Genomsnittligt antal dagar för stängning av affärsmöjlighet (förlorade) | Genomsnittligt antal dagar till en förlorad affärsmöjlighet |
   | Genomsnittligt antal dagar för stängning av affärsmöjlighet (vunnet) | Genomsnittligt antal dagar till en vunnen affärsmöjlighet |
   | Antal alla affärsmöjligheter | Totalt antal alla affärsmöjligheter |
   | Antal affärsmöjligheter (stängda) | Totalt antal stängda affärsmöjligheter (vunna eller förlorade) |
   | Antal affärsmöjligheter (förlorade) | Totalt antal förlorade affärsmöjligheter |
   | Antal affärsmöjligheter (öppna) | Totalt antal öppna affärsmöjligheter |
   | Antal affärsmöjligheter (Won) | Totalt antal möjligheter som vunnits |
   | Affärsmöjlighet - belopp | Totalt affärsmöjlighetsbelopp. Om mer än en lead är associerad med en affärsmöjlighet, baseras allokeringsbeloppet på lead-poäng. |
   | Affärsmöjlighet (förlorad) | Totalt belopp för förlorade affärsmöjligheter. Om mer än en lead är associerad med en affärsmöjlighet, baseras allokeringsbeloppet på lead-poäng. |
   | Belopp för affärsmöjlighet (öppet) | Totalt belopp för öppna affärsmöjligheter. Om mer än en lead är associerad med en affärsmöjlighet, baseras allokeringsbeloppet på lead-poäng. |
   | Belopp för affärsmöjlighet (vunnet) | Totalt belopp för vunna affärsmöjligheter. Om mer än en lead är associerad med en affärsmöjlighet, baseras allokeringsbeloppet på lead-poäng. |

>[!MORELIKETHIS]
>
>* [Skapa en rapport för intäktsutforskaren](create-a-revenue-explorer-report.md)
>* [Lägga till fält i en Intresseutforskarrapport](adding-fields-to-a-revenue-explorer-report.md)
>* [Prenumerera på en rapport om skatteutforskaren](subscribe-to-a-revenue-explorer-report.md)

>



