---
unique-page-id: 2359467
description: E-postprestandarapport - Marketo Docs - produktdokumentation
title: Rapport om e-postprestanda
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Rapport om e-postprestanda {#email-performance-report}

Om du vill se hur bra dina e-postmeddelanden fungerar med status som levererad, öppnad, klickad osv. skapar du en rapport om e-postprestanda.

1. [Skapa en rapport i ett program](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) och välj **[!UICONTROL Email Performance]** [rapporttyp](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Ändra tidsramen för rapporten](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) och klicka på fliken **[!UICONTROL Report]**.
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
   >En rapport om e-postprestanda innehåller aktiviteter för alla personer, inklusive de som har tagits bort sedan e-postmeddelandet skickades. Ibland vill du bara se aktiviteter för aktiva personer. I så fall måste du filtrera bort borttagna personer från rapporten. Använd fliken **[!UICONTROL Smart List]** för att [skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) för rapporten. Om du inte filtrerar något specifikt fält anger du följande som e-postadress: **[!UICONTROL is not empty]**.

   [Välj rapportkolumner](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) för en e-postrapport innehåller:

   <table><thead>

<tr>
    <th>Kolumn</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Hård studsad</td>
    <td>E-postmeddelandet avvisades på grund av ett permanent villkor, t.ex. en e-postadress som inte finns.</td>
  </tr>
  <tr>
    <td>Mjuk studsad</td>
    <td>E-postmeddelandet avvisades på grund av ett tillfälligt villkor, t.ex. att en server är nere eller en fullständig inkorg.</td>
  </tr>
  <tr>
    <td>Väntande</td>
    <td>Det här antalet beräknas genom att subtrahera antalet e-postmeddelanden som levererats, studsat och Mjuk studsade från det totala antalet skickade.</td>
  </tr>
  <tr>
    <td>Klickad länk</td>
    <td>Antal e-postmottagare som klickat på en länk i e-postmeddelandet.</td>
  </tr>
  <tr>
    <td>Avprenumererad</td>
    <td>Antal e-postmottagare som klickat på länken Avbeställ i e-postmeddelandet och fyllt i formuläret.</td>
  </tr>
  <tr>
    <td>Avbruten</td>
    <td>Antal e-postmeddelanden som inte kunde levereras och ingen studshändelse togs emot. Ett e-postmeddelande sägs automatiskt vara avbrutet om inget svar tas emot inom tre dagar från e-postmeddelandet.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Om du klickar på länken för att avbryta prenumerationen och e-postadresserna i ett e-postmeddelande registreras det inte under Länkar som du klickat på i rapporten.

I allmänhet försöker vi använda sunt förnuft för att registrera denna statistik. Om någon till exempel klickade på en länk i ett e-postmeddelande så öppnades e-postmeddelandet tydligt först. Vi följer dessa specifika regler för e-postprestandarapporten:

* **Regel 1**: Varje e-postaktivitetspost är inställd på en, och bara en, av följande: _Levererad_, _Hård studsad_, _Mjuk studsad_ eller _Väntande_.

* **Regel 2**: Om e-postposten visar _[!UICONTROL Opened]_räknas den som_ Levererad _.

* **Regel 3**: Om e-postposten visar _[!UICONTROL Clicked Email]_eller_[!UICONTROL Unsubscribed]_ räknas den som _Levererad_ och _Öppnad_.

* **Regel 4**: Om e-postmeddelandet är _[!UICONTROL Opened]_ignoreras studenterna. Om e-postmeddelandet inte har öppnats har_ Hård studsning _högre prioritet än_ Mjuk studsad _och_ Levererad _.

* **Regel 5**: Om ingen e-postaktivitet tas emot tre dagar efter att den skickades, betraktas den som _Avbruten_.

>[!NOTE]
>
>* Flera utskick från samma kampanj till samma person räknas bara en gång.
>
>* Flera utskick från olika kampanjer till samma person räknas separat.

>[!MORELIKETHIS]
>
>* [Filtrera Assets i e-postrapporter för kampanj](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrera borttagna/sammanfogade poster i en e-postprestandarapport](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Resultatrapport för e-postlänk](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
