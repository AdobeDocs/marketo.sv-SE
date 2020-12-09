---
unique-page-id: 2950578
description: Hantera data i sociala profiler - Marketo Docs - Produktdokumentation
title: Hantera data för social profil
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# Hantera data för social profil {#manage-social-profile-data}

När någon interagerar med en Marketo- [social app](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md), eller auktoriserar sitt sociala nätverk att förifylla ett Marketo-formulär med [social formulärfyllning](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), hämtar Marketo alla data som är tillgängliga från deras sociala profil. Du kan visa den här informationen på sidan [](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)Personinformation eller lägga till den som en kolumn i en [anpassad vy av en smart lista](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List).

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Social formulärfyllning och sociala appar fångar upp lite olika fältuppsättningar, se respektive avsnitt nedan.

>[!NOTE]
>
>**Tillgänglighet**
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
>Data som hämtas av ifyllnad för sociala formulär skriver över matchande fält såvida du inte [blockerar uppdateringar av dessa fält på formulärnivå](../../../../product-docs/administration/field-management/block-updates-to-a-field.md).

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
>Ifyllning av sociala formulär hämtar *endast* e-postadressen om personen skriver in den i formuläret. Om du behöver e-postadressen bör du [göra den till ett obligatoriskt fält i formuläret](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Aktivera ifyllning av [sociala formulär](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)om du vill hämta in den här informationen från formulär.

>[!NOTE]
>
>**Djupdykning**
>
>Läs mer om hur du arbetar med formulär i [Forms](http://docs.marketo.com/display/docs/forms) djupdykning.

