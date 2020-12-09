---
unique-page-id: 9437991
description: Utlösare och filter för smarta mobilkampanjer - Marketo Docs - Produktdokumentation
title: Utlösare och filter för smarta mobilkampanjer
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---


# Utlösare och filter för smarta mobilkampanjer {#triggers-and-filters-for-mobile-smart-campaigns}

Du kan ställa in utlösare och filter för en smart kampanj för mobilappar.

För de flesta aktiviteter finns det en utlösare, ett filter och ett inaktivitetsfilter. Använd inaktivitetsfilter för att spåra en åtgärd som att trycka på ett push-meddelande som *inte* hände.

* Mobilappen är/har installerats
* Mobilappen har öppnats/öppnats
* Har/haft aktivitet för mobilappar
* Har/haft en mobilappssession
* Tryck/tryck på mobilpush-meddelanden

Det finns bara filter för den här aktiviteten:

* Skickades push-meddelande - filter och inaktivitetsfilter

Sök efter **mobilappen** i den högra panelen för att visa alla utlösare och filter för mobilappen.

![](assets/image2015-8-12-17-3a25-3a18.png)

## Begränsningar {#constraints}

Använd begränsningar med utlösare och filter för att ytterligare sortera data.

![](assets/image2015-8-17-12-3a6-3a33.png)

Alla utlösare och filter, förutom för Skickat push-meddelande, innehåller följande två standardbegränsningar:

* Enhetstyp - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, Android smartphone, Android-surfplatta, Okänd (det här är en förinställningslista)

* Plattform - iPhone eller Android

Vissa utlösare och filter har ytterligare begränsningar, till exempel:

* Appversion - Ett sätt att rikta sig till personer som inte har den senaste versionen. Om den senaste programversionen till exempel är 2.0 kan du använda den för att hitta personer som INTE finns i programversion 2.0

* Installationskälla - Det enda alternativet är API

* Språk - Inställningen på enheten

* Mobilapp - Namnet på den specifika appen. Användbar för att ange om du har fler än en

* Plattformsversion - Operativsystemets version

* Sessionslängd (sekunder) - Sessionstid när programmet är i förgrunden

* Är aktiverad - **Sant** innebär att push-meddelanden kan skickas. **Falskt** betyder att de inte kan. personen kan till exempel ha avanmält sig från att ta emot push-meddelanden

## Utlösare och filter {#triggers-and-filters}

**Har mobilapp**

Använd det här filtret för att ta reda på alla som har installerat din app. Det här är bara tillgängligt som ett filter.

>[!NOTE]
>
>Filtret hittar både aktuella och tidigare installationer eftersom Marketo inte spårar programavinstallationer.

**Begränsningar**: Enhetstyp, plattform, mobilapp, mobilappsversion, enhetstyp, installationskälla, är aktiverad och språkinställning

![](assets/image2015-8-21-13-3a33-3a54.png)

>[!TIP]
>
>Det är en god vana att ange Has Mobile App = true och Is Push Enabled = true, samt namnet på din mobilapp när du definierar den smarta listan över vem som ska få ett push-meddelande.

Mobilappen är/har installerats

* Mobilappen är installerad - utlösare

* Mobilappen har installerats - filter

* NOT Mobile App was Installed - inactivity filter

**Begränsningar**: Enhetstyp, plattform, appversion, språk och installationskälla

![](assets/image2015-8-17-13-3a11-3a3.png)

Mobilappen har öppnats/öppnats

* Mobilappen är öppen - utlösare

* Mobilappen öppnades - filter

* NOT Mobile App was Opened - inactivity filter

**Begränsningar**: Enhetstyp och plattform

![](assets/image2015-8-17-13-3a13-3a55.png)

Har/haft aktivitet för mobilappar

Dessa är ett kraftfullt sätt att spåra anpassad mobilaktivitet. Du måste arbeta med utvecklaren för att konfigurera spårning [för Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android) och [för iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Har aktivitet för mobilappar - utlösare

* Har mobilappsaktivitet - filter

* Inte har mobilappsaktivitet - inaktivitetsfilter

**Begränsningar**: Enhetstyp och plattform, plus ytterligare fem:

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
>Här är en mycket specifik åtgärd, med andra begränsningar som definierar den, under åtgärdstypen *Shopping*:
>
>* Köpte en skjorta
>  * Det var rött
>  * Det kostar 30 dollar
>  * Det tog 20 sekunder att köpa


Så här ser filtret ut i Marketo:   ![](assets/image2015-8-17-13-3a16-3a12.png)

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

**Begränsningar**: Enhetstyp, plattform och sessionslängd (sekunder)

![](assets/image2015-8-17-13-3a18-3a34.png)

Tryck/tryck på push-meddelande

* Tryck på push-meddelande - utlösare

* Aktiverat push-meddelande - filter

* Ej aktiverat push-meddelande - inaktivitetsfilter

**Begränsningar**: Enhetstyp, plattform, mobilappsversion, push-meddelande och plattformsversion

![](assets/image2015-8-21-14-3a2-3a24.png)

>[!TIP]
>
>Använd inaktivitetsfiltret Ej påsatt push-meddelande för att hitta personer som inte tryckte på ett push-meddelande som nyligen skickats till dem, så att du kan följa upp via e-post.

**Skickades push-meddelande** Den här aktiviteten är bara tillgänglig som ett filter.

* Skickades push-meddelande - filter

* EJ skickat push-meddelande - inaktivitetsfilter

**Begränsningar**: Push-meddelanden och mobilapp

![](assets/image2015-8-21-14-3a3-3a50.png)

>[!MORELIKETHIS]
>
>* [Lägga till en begränsning i ett smart listfilter](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Använd inaktivitetsfilter i en smart lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

