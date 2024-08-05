---
unique-page-id: 2950578
description: Hantera data i sociala profiler - Marketo Docs - produktdokumentation
title: Hantera data för social profil
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 5%

---

# Hantera data för social profil {#manage-social-profile-data}

När någon interagerar med en Marketo [social app](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md), eller auktoriserar sitt sociala nätverk att förifylla ett Marketo-formulär med [social formulärfyllning](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), hämtar Marketo alla tillgängliga data från sin sociala profil. Du kan visa den här informationen på [personinformationssidan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) eller lägga till den som en kolumn i en [anpassad vy av en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

>[!IMPORTANT]
>
>Den 31 juli 2024 började vi ta bort den här funktionen. Du kommer inte att kunna skapa nya resurser. Befintliga tillgångar kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Social formulärfyllning och sociala appar samlar in lite olika fältuppsättningar. Se respektive avsnitt nedan.

>[!AVAILABILITY]
>
>Alla användare i Marketo Engage har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

## Hämtat via social app {#captured-via-social-app}

Beroende på nätverkets och användarens sekretessinställningar hämtas ett eller flera av dessa fält:

>[!NOTE]
>
>Ytterligare information från sociala nätverk visas på sidan Personinformation ungefär fem minuter efter att personen har auktoriserat.

## Från Twitter: {#from-twitter}

* Förnamn (parsat från visningsnamn)
* Efternamn (parsat från visningsnamn)
* Profilfoto-URL
* Profilsidans URL
* Social räckvidd (antal följare)

>[!NOTE]
>
>Sociala appar hämtar inte personens e-postadress.

## Från Facebook: {#from-facebook}

* Förnamn
* Efternamn
* Profil-URL
* Profilfoto-URL
* Kön
* Social räckvidd (antal vänner)

### Infångad via social formulärfyllning {#captured-via-social-form-fill}

Beroende på nätverkets och användarens sekretessinställningar hämtas ett eller flera av dessa fält:

>[!CAUTION]
>
>Data som hämtas av ifyllning för sociala formulär skriver över matchande fält såvida du inte [blockerar uppdateringar av dessa fält på formulärnivå](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Från Twitter: {#from-twitter-1}

* Förnamn (parsat från visningsnamn)
* Efternamn (parsat från visningsnamn)
* E-post

## Från Facebook: {#from-facebook-1}

* Förnamn
* Efternamn
* E-post
* Födelsedatum
* Befattning
* Företag

>[!NOTE]
>
>Ifyllning av sociala formulär hämtar e-postadressen _endast_ om personen anger den i formuläret. Om du behöver e-postadressen bör du [göra den till ett obligatoriskt fält i formuläret](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Aktivera [fyllning av sociala formulär](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md) om du vill hämta in den här informationen från formulär.
