---
description: Förstå målspårning och projekterade registreringar - Marketo Docs - produktdokumentation
title: Förstå målspårning och projekterade registreringar
exl-id: 110768f4-46ed-4951-96b2-a97813d7b257
feature: Predictive Audiences
source-git-commit: 86f9e9f13b24a82deb50ec4c398035d7d7479d20
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 0%

---

# Förstå målspårning och projekterade registreringar {#understanding-goal-tracking-and-projected-registrations}

Så här ser du hur du kan följa upp dina målframsteg och förstå Marketo prognoser.

>[!PREREQUISITES]
>
>Om du vill ha tillgång till de flesta av dessa funktioner måste du aktivera [nästa generations toggle](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"} för händelseprogram.

>[!NOTE]
>
>När ett händelseprogram skapas i Marketo Classic blir händelsens startdatum som standard det datum då händelsen skapades. Eftersom prognostiserade registreringar tar hänsyn till tiden före en händelses startdatum, kanske dessa nummer inte är korrekta om startdatumet och skapandedatumet är desamma (om de inte anges avsiktligt).

## Målspårning och planerade registreringar

1. Du kan hitta målspårningsinformation på fliken **[!UICONTROL Reports]** i ditt händelseprogram. I just det här exemplet finns det 150 registrerade medlemmar hittills mot målet 200 (75 %).

   ![](assets/understanding-goal-tracking-and-projected-registrations-1.png)

Du kommer också att se dina **[!UICONTROL Projected]**-registreringar. Håll muspekaren över infoikonen om du vill se en uppdelning av det här talet efter segmentet Sannolikhet.

![](assets/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Diagrammet Bifogad och högre förblir tomt tills händelsens dag infaller.

Om du inte har aktiverat växlingsfunktionen visas den här i användargränssnittet för Marketo-klassen:

![](assets/understanding-goal-tracking-and-projected-registrations-3.png)

1. Klicka på knappen Diagram för att växla till en beskrivning av dina medlemmar med sannolikhet för registrering. Aktuella procentsatser för registrering för varje segment, jämfört med den genomsnittliga procentandelen för det segmentet i dina tidigare program.

   ![](assets/understanding-goal-tracking-and-projected-registrations-4.png)

Alla medlemmar (registrerade och ännu inte registrerade) kategoriseras utifrån deras sannolikhet för registrering. Håll muspekaren över informationsikonen för att se hur dessa sannolikhetskategorier definieras.

![](assets/understanding-goal-tracking-and-projected-registrations-5.png)

>[!NOTE]
>
>Prediktionsnumren uppdateras var 24:e timme tills dagen för händelsen. Alla medlemmar som är listade som _Bearbetning_ inkluderas i nästa beräkningscykel.

## Liknande program

Du kan få lite information om ditt aktuella event genom att titta på hur liknande program har utvecklats tidigare. I det här avsnittet visas upp till fem liknande program från de senaste sex månaderna, med antalet/procentandelen medlemmar som var _registrerade_ eller senare.

Vid beräkningen av liknande program har vi bland annat tagit med följande faktorer:

* Programtyp
* Programkanal
* Målgruppsstorlek
* Programtaggar
* Tid från det att händelsen skapas till dess att händelsen startar
* Händelsevaraktighet

  ![](assets/understanding-goal-tracking-and-projected-registrations-6.png)

## Recommendations

Högst upp på sidan [!UICONTROL Reports] kan du hitta AI/ML-drivna rekommendationer baserat på dina framsteg. Ta en titt regelbundet för tips och insikter!

![](assets/understanding-goal-tracking-and-projected-registrations-7.png)

## Personnivåprognoser

Klicka på fliken **[!UICONTROL Members]** för att visa alla programmedlemmar. Håll pekaren över **[!UICONTROL Registration Likelihood]**- eller **[!UICONTROL Attendance Likelihood]**-fälten för att se exakta procentsatser och kategoriseringar. Du kan sedan vidta åtgärder för medlemmar i en viss kategori (t.ex. alla i kategorin&quot;Less Troely&quot; för att registrera) och särskilt inrikta dig på dem för att eventuellt öka antalet.

![](assets/understanding-goal-tracking-and-projected-registrations-8.png)

>[!NOTE]
>
>Individuell sannolikhet tar hänsyn till mer än 40 personfaktorer, inklusive profilattribut, personaktivitet och tidigare inbjuden/registrerade/övervakade aktiviteter.

## Vanliga frågor och svar

**F: Vad är segmentet?**

S: Sannolikheten att registrera är ett värde mellan 0 och 100. Alla som är medlemmar i händelseprogrammet får ett sannolikhetsvärde mellan 0 och 100.

Vi sätter in sannolikhetsvärden i tre segment:

* Sannolikhet att registrera >50 % = segment med mycket sannolikhet
* Sannolikt att registrera >25 % till &lt;50 % = Sannolikt segment
* Sannolikhet för registrering &lt;25% = mindre sannolikhetssegment

När det är troligt att en person registrerar sig hamnar förutsägelsen i ett av dessa segment (alla som är medlemmar i ett program kommer att ingå i ett av dem). Om ett händelseprogram till exempel har 1000 medlemmar baserat på sannolikhetsprognoserna distribueras dessa 1000 till segmenten _Mycket sannolikt_, _Sannolikt_ eller _Mindre troligt_ .

Därför har de som hamnar i segmentet Highly Troely större chans att anmäla sig till evenemanget.

Konvertering till register = # av personer i segment som är registrerade delat med # personer som faller in i segmentet (om till exempel 100 personer faller in i segmentet Mycket sannolikt och 60 av dem registrerar sig, är konverteringsgraden 60 %).

Konvertering % för registrering följer det här mönstret: Mycket sannolikt > Sannolikt > Mindre troligt.

**F: Hur använder jag insikterna?**

S: Bästa praxis innebär följande:

i. Du skapar ett program och sedan använder en Smart Campaign prediktiva filter med &quot;större än X&quot;, vilket skulle resultera i en viss mängd personer (till exempel 1 000) och du kör kampanjen.

ii. Efter 24 timmar kan du på fliken [!UICONTROL Reports] se de planerade registreringarna som beräknas baserat på sannolikheten att registrera värden för alla personer som för närvarande är inbjudna.

iii. Om de planerade registreringarna är mindre än målet måste du bjuda in fler personer. Nu kan du se vilka insikter som visar vilket tröskelvärde som fungerade i tidigare program.

![](assets/understanding-goal-tracking-and-projected-registrations-9.png)

iv. Du kan skapa en ny smart kampanj med det tröskelvärdet för att bjuda in fler personer.

v. När som helst om du vill förstå varför ett projicerat tal visas kan du växla för att se målgruppsfördelningen mellan segment, deras konverteringsgrader från det förflutna och använda konverteringsgraden för den aktuella målgruppen (se skärmbilden nedan).

**Q: Vad är segmenten efter registrering?**

S: Tre staplar, där var och en representerar ett segment (Mycket sannolikt, Sannolikt, Mindre sannolikt).

**Lila prickad linje:** Genomsnittlig konversationsfrekvens för registrering i det segmentet, baserat på tidigare liknande program.

**Blått fält:** Registreringsprocent för alla personer i det segmentet.

![](assets/understanding-goal-tracking-and-projected-registrations-10.png)

Exempel: 100 personer har möjlighet att registrera > 50 % och 60 av dessa 100 personer. Mycket troligt har 60 % konvertering. Det innebär att alla medlemmar som läggs till i programmet är benägna att registrera värden, sedan läggs de in i segment och antalet registrerade personer i varje segmentkonverteringsgrad beräknas.

**F: Vad betyder &quot;Registrerad och högre&quot;?**

S: Alla som är listade som registrerade eller som har en annan status med samma eller högre stegnummer.

Du kan skapa nya statusvärden för ett händelseprogram, men vi mappar dessa statusvärden med standardstatusvärden. Tänk på ett fall där en person flyttas från en inbjudan till en påminnelse, vilket är ett högre steg än registrering. Den här personen betraktas också som registrerad och visas i målspårningen.

![](assets/understanding-goal-tracking-and-projected-registrations-11.png)

**F: Hur beräknas planerade registreringar?**

S: Se nedan.

![](assets/understanding-goal-tracking-and-projected-registrations-12.png)
