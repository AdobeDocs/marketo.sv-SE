---
description: ' [!DNL Veeva] Standardfältmappning - Marketo Docs - produktdokumentation'
title: ' [!DNL Veeva] Standardfältmappning'
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 29%

---

# Standardfältmappning för [!DNL Veeva] {#default-veeva-field-mapping}

När du först synkroniserar ditt Marketo Engage-konto med [!DNL Veeva] skapar Marketo automatiskt dessa associationer mellan dina inbyggda [!DNL Veeva]- och Marketo-fält. Marketo synkroniserar även dina anpassade fält på dina konton och kontakter.

## Kontaktfält {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC</th>
      <th>Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Födelsadatum</td>
      <td>Födelsedatum</td>
    </tr>
    <tr>
      <td>Skapad den</td>
      <td>Skapad av SFDC</td>
    </tr>
    <tr>
      <td>Kontaktbeskrivning</td>
      <td>Personanteckningar</td>
    </tr>
    <tr>
      <td>E-post</td>
      <td>E-postadress</td>
    </tr>
    <tr>
      <td>Fax, arbete</td>
      <td>Faxnummer</td>
    </tr>
    <tr>
      <td>Förnamn</td>
      <td>Förnamn</td>
    </tr>
    <tr>
      <td>Avanmäl dig via e-post</td>
      <td>Avprenumererad</td>
    </tr>
    <tr>
      <td>Borttagen</td>
      <td>SFDC tas bort</td>
    </tr>
    <tr>
      <td>Efternamn</td>
      <td>Efternamn</td>
    </tr>
    <tr>
      <td>Leadkälla</td>
      <td>Källa</td>
    </tr>
    <tr>
      <td>Leadpoäng</td>
      <td>Poäng</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>Ort</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>Land</td>
    </tr>
    <tr>
      <td>Postnummer</td>
      <td>Postnummer</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>Stat</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>Adress</td>
    </tr>
    <tr>
      <td>Mobiltelefon</td>
      <td>Mobiltelefon</td>
    </tr>
    <tr>
      <td>Telefon, arbete</td>
      <td>Telefonnummer</td>
    </tr>
    <tr>
      <td>Titel</td>
      <td>Titel</td>
    </tr>
    <tr>
      <td>Titel</td>
      <td>Befattning</td>
    </tr>
  </tbody>
</table>

## Kontofält {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC</th>
      <th>Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Årlig intäkt</td>
      <td>Årlig intäkt</td>
    </tr>
    <tr>
      <td>Faktureringsort</td>
      <td>Faktureringsort</td>
    </tr>
    <tr>
      <td>Faktureringsland</td>
      <td>Faktureringsland</td>
    </tr>
    <tr>
      <td>Postnummer för fakturering</td>
      <td>Faktureringspostnummer</td>
    </tr>
    <tr>
      <td>Faktureringsstat/provins</td>
      <td>Faktureringsstat</td>
    </tr>
    <tr>
      <td>Faktureringsgatan</td>
      <td>Faktureringsadress</td>
    </tr>
    <tr>
      <td>Kontobeskrivning</td>
      <td>Företagsanteckningar</td>
    </tr>
    <tr>
      <td>Bransch</td>
      <td>Bransch</td>
    </tr>
    <tr>
      <td>Borttagen</td>
      <td>SFDC tas bort</td>
    </tr>
    <tr>
      <td>Kontonamn</td>
      <td>Företagets namn</td>
    </tr>
    <tr>
      <td>Anställda</td>
      <td>Antal anställda</td>
    </tr>
    <tr>
      <td>Telefon till konto</td>
      <td>Telefon</td>
    </tr>
    <tr>
      <td>SNI-kod</td>
      <td>SNI-kod</td>
    </tr>
    <tr>
      <td>Kontowebbplats</td>
      <td>Plats</td>
    </tr>
    <tr>
      <td>Kontotyp</td>
      <td>SFDC Type</td>
    </tr>
    <tr>
      <td>Webbplats</td>
      <td>Webbplats</td>
    </tr>
  </tbody>
</table>

## [!DNL Veeva] relaterade systemfält i Marketo (skrivskyddade) {#veeva-related-system-fields-in-marketo}

Dessa fält skapas i Marketo men kan inte justeras av kunder.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Fält</th>
      <th>Beskrivning</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[!DNL Veeva] ID</td>
      <td>ID:t [!DNL Salesforce] med 18 tecken</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] Typ</td>
      <td>Kontakt. Om det är tomt finns leadet bara som en person i Marketo</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] Skapad den</td>
      <td>Skapad i SFDC (kan skilja sig från Skapad i Marketo)</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] är borttagen</td>
      <td>Tidigare var personen i SFDC men togs bort och bor nu endast i Marketo</td>
    </tr>
  </tbody>
</table>
