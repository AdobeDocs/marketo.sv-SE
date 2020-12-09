---
unique-page-id: 2359467
description: E-postprestandarapport - Marketo Docs - produktdokumentation
title: Rapport om e-postprestanda
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# Rapport om e-postprestanda {#email-performance-report}

Om du vill se hur bra dina e-postmeddelanden fungerar med status som levererad, öppnad, klickad osv. skapar du en rapport om e-postprestanda.

1. [Skapa en rapport i ett program](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) och välj **E-postresultatets** [rapporttyp](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Ändra tidsramen](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) för rapporten och klicka på fliken **Rapport** .
1. Du är där! Utforska nu rapporten och se hur dina e-postmeddelanden har fungerat.

   >[!NOTE]
   >
   >Filtret Skickat baseras på det första datumet som e-postmeddelandet skickades.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Klicka på namnet på ett e-postmeddelande för att öppna det i E-postförhandsgranskaren.

   >[!NOTE]
   >
   >
   >En rapport om e-postprestanda innehåller aktiviteter för alla personer, inklusive de som har tagits bort sedan e-postmeddelandet skickades. Ibland vill du bara se aktiviteter för aktiva personer. I så fall måste du filtrera bort borttagna personer från rapporten. Använd fliken **Smart lista** för att [skapa en smart lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) för rapporten. Om du inte filtrerar något specifikt fält anger du följande för e-postadressfiltret: **är inte tom**.

   [Välj Rapportkolumner](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) för en e-postrapport som innehåller:

   | Kolumn | Beskrivning |
   |---|---|
   | Hård studsad | E-postmeddelandet avvisades på grund av ett permanent villkor, t.ex. en e-postadress som inte finns. |
   | Mjuk studsad | E-postmeddelandet avvisades på grund av ett tillfälligt villkor, t.ex. att en server är nere eller en fullständig inkorg. |
   | Väntande | Det här antalet beräknas genom att subtrahera antalet e-postmeddelanden som levererats, studsat och Mjuk studsade från det totala antalet skickade. |
   | Klickad länk | Antal e-postmottagare som klickat på en länk i e-postmeddelandet. |
   | Avbeställ | Antal e-postmottagare som klickat på länken **Avbeställ** i e-postmeddelandet och fyllt i formuläret. |

   >[!NOTE]
   >
   >Om du klickar på länken för att avbryta prenumerationen och e-postadresserna i ett e-postmeddelande registreras det inte under Länkar som du klickat på i rapporten.

I allmänhet försöker vi använda sunt förnuft för att registrera denna statistik. Om någon till exempel klickade på en länk i ett e-postmeddelande så öppnades e-postmeddelandet tydligt först. Vi följer dessa specifika regler för e-postprestandarapporten:

* **Regel 1**: Varje post för e-postaktivitet anges till en, och bara en, av följande: *Levererad*, *Hård studsad*, *Mjuk studsad* eller *Väntande*.

* **Regel 2**: Om e-postposten visar *Öppnad* räknas den som *Levererad*.

* **Regel 3**: Om e-postposten visar *klickad e-post* eller *Avbeställ* räknas den som *Levererad* och *Öppnad*.

* **Regel 4**: Om e-postmeddelandet är *öppet* ignoreras studenterna. Om e-postmeddelandet inte har öppnats har *Hård* studsning företräde framför *Mjuk studsad* och *Levererad*.

>[!NOTE]
>
>Flera utskick från samma kampanj till samma person räknas bara en gång.

>[!MORELIKETHIS]
>
>* [Filtrera resurser i e-postrapporter för kampanj](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Resultatrapport för e-postlänk](email-link-performance-report.md)

>



>[!NOTE]
>
>**Djupdykning**
>
>Läs mer i [Grundläggande rapportering](http://docs.marketo.com/display/docs/basic+reporting).

