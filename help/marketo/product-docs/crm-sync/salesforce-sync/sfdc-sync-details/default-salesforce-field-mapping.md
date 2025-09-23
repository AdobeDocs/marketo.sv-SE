---
unique-page-id: 4719314
description: Standardfältmappning för Salesforce - Marketo Docs - produktdokumentation
title: Standardfältmappning för Salesforce
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Standardfältmappning för [!DNL Salesforce] {#default-salesforce-field-mapping}

När du först synkroniserar ditt Marketo Engage-konto med Salesforce skapar Marketo automatiskt dessa associationer mellan de inbyggda fälten i Salesforce och Marketo. Marketo synkroniserar även dina anpassade fält på leads, konton, säljprojekt och kontakter.

## Leadfält {#lead-fields}

| SFDC | Marketo |
|---|---|
| [!UICONTROL Annual Revenue] | [!UICONTROL Annual Revenue] |
| [!UICONTROL City] | [!UICONTROL City] |
| [!UICONTROL Company] | [!UICONTROL Company Name] |
| [!UICONTROL Converted Date] | [!UICONTROL SFDC Converted Date] |
| [!UICONTROL Country] | [!UICONTROL Country] |
| [!UICONTROL Created Date] | [!UICONTROL SFDC Created Date] |
| [!UICONTROL Description] | [!UICONTROL Person Notes] |
| [!UICONTROL Email] | [!UICONTROL Email Address] |
| [!UICONTROL Fax] | [!UICONTROL Fax Number] |
| [!UICONTROL First Name] | [!UICONTROL First Name] |
| [!UICONTROL Email Opt Out] | [!UICONTROL Unsubscribed] |
| [!UICONTROL Industry] | [!UICONTROL Industry] |
| [!UICONTROL Converted] | [!UICONTROL SFDC Is Converted] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Last Name] | [!UICONTROL Last Name] |
| [!UICONTROL Lead Source] | [!UICONTROL Source] |
| [!UICONTROL Lead Score] | [!UICONTROL Score] |
| [!UICONTROL Mobile Phone] | [!UICONTROL Mobile Phone Number] |
| [!UICONTROL Employees] | [!UICONTROL Num Employees] |
| [!UICONTROL Phone] | [!UICONTROL Phone Number] |
| [!UICONTROL Zip/Postal Code] | [!UICONTROL Postal Code] |
| [!UICONTROL Rating] | [!UICONTROL Rating] |
| [!UICONTROL Salutation] | [!UICONTROL Salutation] |
| [!UICONTROL State/Province] | [!UICONTROL State] |
| [!UICONTROL Status] | [!UICONTROL Status] |
| [!UICONTROL Street] | [!UICONTROL Address] |
| [!UICONTROL Title] | [!UICONTROL Job Title] |
| [!UICONTROL Website] | [!UICONTROL Website] |

## Kontaktfält {#contact-fields}

| SFDC | Marketo |
|---|---|
| [!UICONTROL Birthdate] | [!UICONTROL Date of Birth] |
| [!UICONTROL Created Date] | [!UICONTROL SFDC Created Date] |
| [!UICONTROL Contact Description] | [!UICONTROL Person Notes] |
| [!UICONTROL Email] | [!UICONTROL Email Address] |
| [!UICONTROL Business Fax] | [!UICONTROL Fax Number] |
| [!UICONTROL First Name] | [!UICONTROL First Name] |
| [!UICONTROL Email Opt Out] | [!UICONTROL Unsubscribed] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Last Name] | [!UICONTROL Last Name] |
| [!UICONTROL Lead Source] | [!UICONTROL Source] |
| [!UICONTROL Lead Score] | [!UICONTROL Score] |
| [!UICONTROL MailingCity] | [!UICONTROL City] |
| [!UICONTROL MailingCountry] | [!UICONTROL Country] |
| [!UICONTROL MailingPostalCode] | [!UICONTROL Postal Code] |
| [!UICONTROL MailingState] | [!UICONTROL State] |
| [!UICONTROL MailingStreet] | [!UICONTROL Address] |
| [!UICONTROL Mobile Phone] | [!UICONTROL Mobile Phone Number] |
| [!UICONTROL Business Phone] | [!UICONTROL Phone Number] |
| [!UICONTROL Salutation] | [!UICONTROL Salutation] |
| [!UICONTROL Title] | [!UICONTROL Job Title] |

## Kontofält {#account-fields}

| [!UICONTROL SFDC field] | [!UICONTROL Marketo field] |
|---|---|
| [!UICONTROL Annual Revenue] | [!UICONTROL Annual Revenue] |
| [!UICONTROL Billing City] | [!UICONTROL Billing City] |
| [!UICONTROL Billing Country] | [!UICONTROL Billing Country] |
| [!UICONTROL Billing Zip/Postal Code] | [!UICONTROL Billing Postal Code] |
| [!UICONTROL Billing State/Province] | [!UICONTROL Billing State] |
| [!UICONTROL Billing Street] | [!UICONTROL Billing Address] |
| [!UICONTROL Account Description] | [!UICONTROL Company Notes] |
| [!UICONTROL Industry] | [!UICONTROL Industry] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Account Name] | [!UICONTROL Company Name] |
| [!UICONTROL Employees] | [!UICONTROL Num Employees] |
| [!UICONTROL Account Phone] | [!UICONTROL Main Phone] |
| [!UICONTROL SIC Code] | [!UICONTROL SIC Code] |
| [!UICONTROL Account Site] | [!UICONTROL Site] |
| [!UICONTROL Account Type] | [!UICONTROL SFDC Type] |
| [!UICONTROL Website] | [!UICONTROL Website] |

## [!DNL Salesforce] relaterade systemfält i Marketo (skrivskyddade) {#salesforce-related-system-fields-in-marketo-read-only}

Dessa fält skapas i Marketo men kan inte justeras av kunder.

| Fält | Beskrivning |
|---|---|
| SFDC ID | ID:t [!DNL Salesforce] med 18 tecken |
| SFDC Type | Lead eller kontakt. Om det är tomt finns leadet bara som en person i Marketo |
| Skapad av SFDC | Skapad i SFDC (kan skilja sig från Skapad i Marketo) |
| SFDC tas bort | Tidigare var personen i SFDC men togs bort och bor nu endast i Marketo |
