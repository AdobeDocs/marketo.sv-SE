---
unique-page-id: 9437991
description: Utlösare och filter för smarta mobilkampanjer - Marketo Docs - produktdokumentation
title: Utlösare och filter för smarta mobilkampanjer
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
source-git-commit: a90f752b291e6d34c920a94795011a8c9efa6d5b
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Utlösare och filter för smarta mobilkampanjer {#triggers-and-filters-for-mobile-smart-campaigns}

Du kan ställa in utlösare och filter för en smart kampanj för mobilappar.

För de flesta aktiviteter finns det en utlösare, ett filter och ett inaktivitetsfilter. Använd inaktivitetsfilter för att spåra en åtgärd, som att trycka på ett push-meddelande, som *inte* inträffar.

* Mobilappen är/har installerats
* Mobilappen har öppnats/öppnats
* Har/haft aktivitet för mobilappar
* Har/haft en mobilappssession
* Tryck/tryck på mobilpush-meddelanden

Det finns bara filter för den här aktiviteten:

* Skickades push-meddelande - filter och inaktivitetsfilter

Sök efter **mobilapp** i den högra panelen för att lista alla mobilappsutlösare och -filter.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Begränsningar {#constraints}

Använd begränsningar med utlösare och filter för att ytterligare sortera data.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Alla utlösare och filter, förutom för Skickat push-meddelande, innehåller följande två standardbegränsningar:

* Enhetstyp - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, Android-smarttelefon, Android-surfplatta, Okänd (det här är en förinställningslista)

* Plattform - iPhone eller Android

Vissa utlösare och filter har ytterligare begränsningar, till exempel:

* Appversion - Ett sätt att rikta sig till personer som inte har den senaste versionen. Om den senaste programversionen till exempel är 2.0 kan du använda den för att hitta personer som INTE finns i programversion 2.0

* Installationskälla - Det enda alternativet är API

* Språk - Inställningen på enheten

* Mobilapp - Namnet på den specifika appen. Användbar för att ange om du har fler än en

* Plattformsversion - Operativsystemets version

* Sessionslängd (sekunder) - Sessionstid när programmet är i förgrunden

* Är push-aktiverad - **True** innebär att push-meddelanden kan skickas. **Falskt** betyder att de inte kan det, personen kan till exempel ha avanmält sig från att ta emot push-meddelanden

## Utlösare och filter {#triggers-and-filters}

**Har mobilapp**

Använd det här filtret för att ta reda på alla som har installerat din app. Det här är bara tillgängligt som ett filter.

>[!NOTE]
>
>Filtret hittar både aktuella och tidigare installationer eftersom Marketo inte spårar programavinstallationer.

**Begränsningar** - Enhetstyp, plattform, mobilapp, mobilappsversion, enhetstyp, installationskälla, är aktiverad och språkinställning

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>Det är en god vana att ange Has Mobile App = true och Is Push Enabled = true, samt namnet på din mobilapp när du definierar den smarta listan över vem som ska få ett push-meddelande.

Mobilappen är/har installerats

* Mobilappen är installerad - utlösare

* Mobilappen har installerats - filter

* NOT Mobile App was Installed - inactivity filter

**Begränsningar** - Enhetstyp, plattform, appversion, språk och installationskälla

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

Mobilappen har öppnats/öppnats

* Mobilappen är öppen - utlösare

* Mobilappen öppnades - filter

* NOT Mobile App was Opened - inactivity filter

**Begränsningar** - Enhetstyp och plattform

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Har/haft aktivitet för mobilappar

Dessa är ett kraftfullt sätt att spåra anpassad mobilaktivitet. Du måste arbeta med utvecklaren för att ställa in spårning [för Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android) och [för iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Har aktivitet för mobilappar - utlösare

* Har mobilappsaktivitet - filter

* Inte har mobilappsaktivitet - inaktivitetsfilter

**Begränsningar** - Enhetstyp, plattform, mobilappsversion, språkområde, plattformsversion plus ytterligare fem:

* Åtgärd - Anpassad mobilaktivitet

* Åtgärdstyp - (valfritt) Textfält som används för att kategorisera flera åtgärder

* Åtgärdsinformation - (valfritt) Textfält som innehåller ytterligare information om en åtgärd

* Åtgärdsmått - (valfritt) Numeriskt fält som innehåller ytterligare information om en åtgärd (till exempel pris)

* Åtgärdslängd (sekunder) - (valfritt) Numeriskt fält som kan användas för att ta reda på hur lång tid det tog för användaren att slutföra en åtgärd

Med åtgärdsbegränsningarna kan du använda utlösaren och filtren för att spåra mobilaktivitet mycket noga.

>[!NOTE]
>
>**Exempel**
>
>Under åtgärdstypen för *Shopping*, här är en mycket specifik åtgärd med andra begränsningar som definierar den:
>
>* Köpte en skjorta
   >   * Det var rött
   >   * Det kostar 30 dollar
   >   * Det tog 20 sekunder att köpa


Så här ser filtret ut i Marketo:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Exempel**
>
>Du kan ha flera åtgärder under samma åtgärdstyp. Faktum är att din normala shoppingupplevelse kan omfatta flera kolumner under Shopping! Skulle det smaka med strumporna?
>
>| Åtgärdstyp | Shopping | Shopping |
>|---|---|---|
>| Åtgärd | Skämt skjorta | Köpta byxor |
>| Åtgärdsinformation | Färg | Färg |
>| Åtgärdsmått | Pris | Pris |


**Har/haft en mobilappssession**

* Har mobilappssession - utlösare

* Hade mobilappssession - filter

* Inte hade mobilappssession - inaktivitetsfilter

**Begränsningar** - Enhetstyp, plattform och sessionslängd (sekunder)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Tryck/tryck på push-meddelande

* Tryck på push-meddelande - utlösare

* Aktiverat push-meddelande - filter

* Ej aktiverat push-meddelande - inaktivitetsfilter

**Begränsningar** - Enhetstyp, plattform, mobilappsversion, push-meddelanden och plattformsversion

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Använd inaktivitetsfiltret Ej påsatt push-meddelande för att hitta personer som inte tryckte på ett push-meddelande som nyligen skickats till dem, så att du kan följa upp via e-post.

**Har skickat push-meddelande** Den här aktiviteten är bara tillgänglig som ett filter.

* Skickades push-meddelande - filter

* EJ skickat push-meddelande - inaktivitetsfilter

**Begränsningar** - Push-meddelanden och mobilapp

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Lägga till en begränsning i ett smart listfilter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Använd inaktivitetsfilter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

