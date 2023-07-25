---
unique-page-id: 2359467
description: E-postprestandarapport - Marketo Docs - produktdokumentation
title: Rapport om e-postprestanda
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Rapport om e-postprestanda {#email-performance-report}

Om du vill se hur bra dina e-postmeddelanden fungerar med status som levererad, öppnad, klickad osv. skapar du en rapport om e-postprestanda.

1. [Skapa en rapport i ett program](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) och väljer **E-postprestanda** [Typ av rapportering](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Ändra tidsramen för rapporten](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) och klicka på **Rapport** -fliken.
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
   >En rapport om e-postprestanda innehåller aktiviteter för alla personer, inklusive de som har tagits bort sedan e-postmeddelandet skickades. Ibland vill du bara se aktiviteter för aktiva personer. I så fall måste du filtrera bort borttagna personer från rapporten. Använd **Smart List** tabba till [skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) för rapporten. Om du inte filtrerar något specifikt fält anger du följande för e-postadressfiltret: **är inte tom**.

   [Välj rapportkolumner](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) för en rapport om e-postprestanda inkluderar:

   | Kolumn | Beskrivning |
   |---|---|
   | Hård studsad | E-postmeddelandet avvisades på grund av ett permanent villkor, t.ex. en e-postadress som inte finns. |
   | Mjuk studsad | E-postmeddelandet avvisades på grund av ett tillfälligt villkor, t.ex. att en server är nere eller en fullständig inkorg. |
   | Väntande | Det här antalet beräknas genom att subtrahera antalet e-postmeddelanden som levererats, studsat och Mjuk studsade från det totala antalet skickade. |
   | Klickad länk | Antal e-postmottagare som klickat på en länk i e-postmeddelandet. |
   | Avprenumererad | Antal e-postmottagare som klickade på **Avbeställ** i e-postmeddelandet och ifyllt formuläret. |

   >[!NOTE]
   >
   >Om du klickar på länken för att avbryta prenumerationen och e-postadresserna i ett e-postmeddelande registreras det inte under Länkar som du klickat på i rapporten.

I allmänhet försöker vi använda sunt förnuft för att registrera denna statistik. Om någon till exempel klickade på en länk i ett e-postmeddelande så öppnades e-postmeddelandet tydligt först. Vi följer dessa specifika regler för e-postprestandarapporten:

* **Regel 1**: Varje post för e-postaktivitet anges till en, och bara en, av följande: _Levererat_, _Hård studsad_, _Mjuk studsad_, eller _Väntande_.

* **Regel 2**: Om e-postposten visas *Öppnad*, räknas det som *Levererat*.

* **Regel 3**: Om e-postposten visas _E-post som klickades_ eller _Avbeställ_, räknas det som _Levererat_ och _Öppnad_.

* **Regel 4**: Om e-postadressen är _Öppnad_, studsar ignoreras. Om e-postmeddelandet inte har öppnats _Hård studsad_ har företräde framför _Mjuk studsad_ och _Levererat_.

>[!NOTE]
>
>Flera skicka från samma kampanj till samma person räknas bara en gång.

>[!MORELIKETHIS]
>
>* [Filtrera resurser i e-postrapporter för kampanj](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Resultatrapport för e-postlänk](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
