---
unique-page-id: 2953415
description: Använda personinformationssidan - Marketo Docs - produktdokumentation
title: Använda personinformationssidan
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 13%

---

# Använda personinformationssidan {#using-the-person-detail-page}

Personinformationssidan innehåller all information som Marketo känner till om en person. Du kan redigera data direkt från den här sidan.

## Komma till personinformationssidan {#getting-to-person-detail-page}

Det finns många sätt att öppna specifika personer. Några exempel är:

* Från **Databas** kan du söka i Snabbsökning
* Valfri smart **list** eller lista
* **Medlemmar** flik i ett program
* **Visa kampanjmedlemmar** i en smart kampanj
* Några **rapporter**

   <br> 

1. Dubbelklicka på en person eller klicka en gång på ID:t till vänster.

   ![](assets/one-1.png)

1. Detta öppnar skärmen för personinformation.

   ![](assets/two-5.png)

## Sidorganisation - Salesforce {#page-organization-salesforce}

Personinformation kategoriseras på följande flikar:

| Tabb | Beskrivning |
|---|---|
| Info | Kontaktinformation och anpassade fält om en person. |
| Företagsinformation | Personens företagsinformation och adress. |
| Information om affärsmöjlighet | Information om affärsmöjlighet synkroniserad från Salesforce. |
| SFDC-huvudfält | Inbyggda Salesforce-fält. |
| SFDC anpassat fält | Anpassade Salesforce-fält. |
| Aktivitetslogg | Alla aktiviteter som rör personen. |

## Sidorganisation - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tabb | Beskrivning |
|---|---|
| Info | Kontaktinformation och anpassade fält om en person. |
| Företagsinformation | Personens företagsinformation och adress. |
| Information om affärsmöjlighet | Information om affärsmöjlighet synkroniserad från Microsoft. |
| Microsoft anpassade fält | Anpassade Microsoft-fält. |
| Microsoft Lead Field | Inbyggda Microsoft-fält. |
| Aktivitetslogg | Alla aktiviteter som rör personen. |

>[!NOTE]
>
>Du kan även se information om säljprojekt [infogat via API](https://developers.marketo.com/rest-api/lead-database/opportunities/) för instanser som inte har synkroniserats med en CRM.

## Redigera ett fält {#editing-a-field}

Många fält kan redigeras. Om du vill uppdatera en persons information skriver du in ett nytt värde och klickar utanför fältet för att spara.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Marketo-standardfält före CRM-synkronisering {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Adress | Årlig intäkt | Anonym IP | Faktureringsadress | Faktureringsort |
| Faktureringsland | Faktureringspostnummer | Faktureringsstat | Ort | Företagets namn |
| Land | Skapad den | Födelsedatum | Avdelning | Ring inte |
| Anropa inte orsak | Orsak till ring inte | E-postadress | Ogiltig e-postadress | Ogiltig e-postorsak |
| ID för externt företag | ID för extern säljare | Faxnummer | Förnamn | Fullständigt namn |
| Bransch | Inaktuell ort | Berört företag | Berört land | Ingående metropolitområde |
| Riktnummer för inkommande telefon | Infört postnummer | Ingångsregion | Är anonym | Är kund |
| Är partner | Befattning | Efternamn | Klassificering | Poäng |
| Personkälla | Status | Telefon | Marketo Social Facebook Display Name | Marketo Social Facebook ID |
| Marketo Social Facebook Photo URL | Marketo Social Facebook Profile URL | Marketo Social Facebook Reach | Refererade registreringar från Marketo Social Facebook | Refererade Marketo Social Facebook-besök |
| Marketo Social Genus | Marketo Social, senast refererad registrering | Marketo Social, senaste refererat besök | Marketo Social LinkedIn Display Name | Marketo Social LinkedIn ID |
| Marketo Social LinkedIn Photo URL | Marketo Social LinkedIn Profile URL | Marketo Social LinkedIn Reach | Refererade registreringar från Marketo Social LinkedIn | Refererade Marketo Social LinkedIn-besök |
| Marketo Social Syndication ID | Marketo Social, totalt antal refererade registreringar | Marketo Social, totalt antal refererade besök | Marketo Social Twitter Display Name | Marketo Social Twitter ID |
| Marketo Social Twitter Photo URL | Marketo Social Twitter Profile URL | Marketo Social Twitter Reach | Refererade registreringar från Marketo Social Twitter | Refererade Marketo Social Twitter-besök |
| Mellannamn | Mobiltelefon | Antal anställda | Telefonnummer | Postnummer |
| Prioritet | Relativa poäng | Roll | Titel | SNI-kod |
| Plats | Stat | Avprenumererad | Orsak till avprenumeration | Uppdaterat den |
| Akut | Webbplats |  |  |  |

>[!NOTE]
>
>Vissa fält är _not_ redigerbar:
>
>* Aktivitetslogg
>* Företagsinformation
>* Möjligheter för SFDC-kontakter
>* Vissa Marketo-specifika fält, t.ex. Skapad och Ursprunglig källtyp.
>
>Läs mer om [Systemhanterade fält](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Skapa en anpassad flik för personinformationssidan](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
