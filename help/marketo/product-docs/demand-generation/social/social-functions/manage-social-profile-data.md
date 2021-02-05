---
unique-page-id: 2950578
description: Hantera data i sociala profiler - Marketo Docs - Produktdokumentation
title: Hantera data för social profil
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Hantera data för social profil {#manage-social-profile-data}

När någon interagerar med en Marketo [social app](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md), eller auktoriserar sitt sociala nätverk att förifylla ett Marketo-formulär med [ifyllnad av sociala formulär](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), hämtar Marketo alla data som är tillgängliga från deras sociala profil. Du kan visa den här informationen på [personinformationssidan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md), eller lägga till den som en kolumn i en [anpassad vy av en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

Social formulärfyllning och sociala appar fångar upp lite olika fältuppsättningar, se respektive avsnitt nedan.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

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
>Data som hämtas av ifyllnad för sociala formulär skriver över matchande fält såvida du inte [blockerar uppdateringar av dessa fält på formulärnivå](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

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
>Ifyllning av sociala formulär hämtar endast e-postadressen _om personen skriver in den i formuläret._ Om du behöver e-postadressen ska du [göra den till ett obligatoriskt fält i formuläret](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Aktivera [ifyllning av sociala formulär](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md) om du vill hämta in den här informationen från formulär.
