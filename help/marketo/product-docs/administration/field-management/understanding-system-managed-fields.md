---
unique-page-id: 5472615
description: Om systemhanterade fält - Marketo Docs - produktdokumentation
title: Förstå systemhanterade fält
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---

# Förstå systemhanterade fält {#understanding-system-managed-fields}

Du kan ha lagt märke till att [personinformationssidan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} innehåller en serie fält som inte kan redigeras och som har skapats av Marketo. Dessa data kommer från olika källor och det finns otaliga värden som kan visas.

## Fälttyper {#field-types}

<table><thead>
  <tr>
    <th>Fältnamn</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ursprunglig Source-typ</td>
    <td>Den plats där en person eller en besökare på webbplatsen först upptäcktes (Exempel: Listimport, Webbsidesbesök)</td>
  </tr>
  <tr>
    <td>Ursprunglig Source-information</td>
    <td>Specifikationer om den platsen (Exempel: listans namn, webbsidans URL)</td>
  </tr>
  <tr>
    <td>Ursprunglig sökmotor</td>
    <td>Om tillämpligt, sökmotorn som refererade personen till den ursprungliga källan</td>
  </tr>
  <tr>
    <td>Ursprunglig sökfras</td>
    <td>Om tillämpligt, det sökord som refererade personen till den ursprungliga inmatningskällan</td>
  </tr>
  <tr>
    <td>Ursprunglig referens</td>
    <td>URL som var värd för den ursprungliga inmatningskällan</td>
  </tr>
  <tr>
    <td>Registrera Source Type</td>
    <td>Den plats där en aktivitet först blev en person (Exempel: Listimport, Webbsidesbesök)</td>
  </tr>
  <tr>
    <td>Registrera Source Info</td>
    <td>Specifikationer om den platsen (Exempel: listans namn, webbsidans URL)</td>
  </tr>
  <tr>
    <td>Anonym IP</td>
    <td>Anger en persons IP-adress</td>
  </tr>
  <tr>
    <td>Berört företag</td>
    <td>Marketo bästa gissning (baserat på IP) för personens företag</td>
  </tr>
  <tr>
    <td>Inaktuell ort</td>
    <td>Marketo bästa gissning (baserat på IP) för personens ort</td>
  </tr>
  <tr>
    <td>Ingångsregion</td>
    <td>Marketo bästa gissning (baserat på IP) för personens stat eller region</td>
  </tr>
  <tr>
    <td>Infört postnummer</td>
    <td>Marketo bästa gissning (baserat på IP) för personens postnummer</td>
  </tr>
  <tr>
    <td>Berört land</td>
    <td>Marketo bästa gissning (baserat på IP) för personens land</td>
  </tr>
  <tr>
    <td>Ingående metropolitområde</td>
    <td>Marketo bästa gissning (baserat på IP) för personens storstadsområde</td>
  </tr>
  <tr>
    <td>Riktnummer för inkommande telefon</td>
    <td>Marketo bästa gissning (baserat på IP) för personens riktnummer</td>
  </tr>
</tbody></table>

## Möjliga värden för Source-typen Original och Registration {#possible-values-for-original-and-registration-source-type}

Nedan finns några möjliga värden och vad de betyder.

<table><thead>
  <tr>
    <th>Ursprunglig Source-typ</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>En person upptäcktes från Salesforce-synkroniseringen</td>
  </tr>
  <tr>
    <td>Webbsidesbesök</td>
    <td>En person upptäcktes från en webbsida</td>
  </tr>
  <tr>
    <td>Fylla i webbformulär</td>
    <td>En person upptäcktes när ett formulär fylldes i</td>
  </tr>
  <tr>
    <td>Listimport</td>
    <td>Personen upptäcktes från en listimport</td>
  </tr>
  <tr>
    <td>Ny person</td>
    <td>Personen har angetts manuellt i databasen</td>
  </tr>
  <tr>
    <td>Klicka på webblänk</td>
    <td>Personen upptäcktes efter att ha klickat på en länk</td>
  </tr>
  <tr>
    <td>E-postadress</td>
    <td>Personen fick ett e-postmeddelande via e-posttillägget Sales Insight</td>
  </tr>
  <tr>
    <td>Person</td>
    <td>Personen synkroniserades från Salesforce som en person</td>
  </tr>
  <tr>
    <td>Kontakt</td>
    <td>Personen synkroniserades från Webkrok som en kontakt</td>
  </tr>
  <tr>
    <td>MUNCHKIN API</td>
    <td>Personen upptäcktes av Marketo Engage Munchkin API</td>
  </tr>
  <tr>
    <td>Social app</td>
    <td>Personen upptäcktes av en social widget</td>
  </tr>
  <tr>
    <td>Webbtjänstens API</td>
    <td>Personen upptäcktes av ett webbtjänste-API</td>
  </tr>
  <tr>
    <td>Evenemangspartner</td>
    <td>Personen upptäcktes via en synkroniserad webbinatjänst</td>
  </tr>
  <tr>
    <td>Associera lead</td>
    <td>Person som har slagits samman via Associate Lead API-anrop</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>Registrera Source Type</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Listimport</td>
    <td>Bli en person genom en listimport</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Bli en person via Salesforce-synkronisering</td>
  </tr>
  <tr>
    <td>Fylla i webbformulär</td>
    <td>Bli en person efter att ha fyllt i ett formulär</td>
  </tr>
  <tr>
    <td>E-postadress</td>
    <td>Personen fick ett e-postmeddelande via e-posttillägget Sales Insight</td>
  </tr>
  <tr>
    <td>Webbtjänstens API</td>
    <td>Personen skapades via SOAP/REST API</td>
  </tr>
  <tr>
    <td>Ny person</td>
    <td>Personen har angetts manuellt i databasen</td>
  </tr>
  <tr>
    <td>MUNCHKIN API</td>
    <td>Bli en person med Marketo Munchkin API</td>
  </tr>
  <tr>
    <td>Social app</td>
    <td>Bli en person via en social widget</td>
  </tr>
  <tr>
    <td>Evenemangspartner</td>
    <td>Bli en person via en länkad webbinatjänst</td>
  </tr>
</tbody>
</table>
