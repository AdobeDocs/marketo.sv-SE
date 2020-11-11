---
title: understanding-target-tracking-and-projicerad-registreringar
description: Förstå målspårning och projekterade registreringar
translation-type: tm+mt
source-git-commit: 1231bc32a3abdf66c10864d6605234763618dbe0
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---


# Förstå målspårning och projekterade registreringar

<br> 

När du har [ställt in händelsemål](/help/sky/setting-event-goals.md)och skickat ut inbjudningar via en [smart kampanj](/help/sky/create-a-smart-campaign.md), så här spårar du målförloppet och förstår Marketos prognoser.

>[!NOTE]
>
>När ett händelseprogram skapas i Marketo Classic blir händelsens startdatum som standard det datum då händelsen skapades. Eftersom prognostiserade registreringar tar hänsyn till tiden före en händelses startdatum, kanske dessa nummer inte är korrekta om startdatumet och skapandedatumet är desamma (om de inte anges avsiktligt).

## Målspårning och planerade registreringar

1. Du hittar målspårningsinformation på fliken [!UICONTROL **Rapporter**] i ditt händelseprogram. I just det här exemplet finns det 150 registrerade medlemmar hittills mot målet 200 (75 %).

   ![Bild ett](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

Du kommer också att se dina [!UICONTROL **planerade**] registreringar. Håll muspekaren över infoikonen om du vill se en uppdelning av det här talet efter segmentet Sannolikhet.

![Bild två](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Diagrammet Bifogad och högre förblir tomt tills händelsens dag infaller.

1. Klicka på knappen Diagram för att växla till en beskrivning av dina medlemmar med sannolikhet för registrering. Aktuella procentsatser för registrering för varje segment, jämfört med den genomsnittliga procentandelen för det segmentet i dina tidigare program.

   ![Bild tre](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

Alla medlemmar (registrerade och ännu inte registrerade) kategoriseras utifrån deras sannolikhet för registrering. Håll muspekaren över informationsikonen för att se hur dessa sannolikhetskategorier definieras.

![Bild fyra](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Prediktionsnumren uppdateras var 24:e timme tills dagen för händelsen. Alla medlemmar som anges som _Bearbetning_ inkluderas i nästa beräkningscykel.

## Liknande program

Du kan få lite information om ditt aktuella event genom att titta på hur liknande program har utvecklats tidigare. I det här avsnittet visas upp till fem liknande program från de senaste sex månaderna, med antalet/procentandelen medlemmar som var _registrerade_ eller högre.

Vid beräkningen av liknande program har vi bland annat tagit med följande faktorer:

* Programtyp
* Programkanal
* Målgruppsstorlek
* Programtaggar
* Tid från det att händelsen skapas till dess att händelsen startar
* Händelsevaraktighet

   ![Bild fem](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

Högst upp på sidan Rapporter hittar du AI/ML-drivna rekommendationer baserat på dina framsteg. Ta en titt regelbundet för tips och insikter!

![Bild sex](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## Personnivåprognoser

Klicka på fliken [!UICONTROL **Medlemmar**] för att visa alla programmedlemmar. Håll muspekaren över fälten [!UICONTROL **Registreringssannolikhet**] eller [!UICONTROL **Närvaro**] för att se exakta procentsatser och kategoriseringar. Du kan sedan vidta åtgärder för medlemmar i en viss kategori (t.ex. alla i kategorin&quot;Less Troely&quot; för att registrera) och särskilt inrikta dig på dem för att eventuellt öka dina registreringsnummer.

![Bild sju](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>Individuell sannolikhet tar hänsyn till mer än 40 personfaktorer, inklusive profilattribut, personaktivitet och tidigare inbjuden/registrerade/övervakade aktiviteter.

## Vanliga frågor

**F: Vad är segmentet?**

S: Sannolikt att registrera är ett värde mellan 0 och 100. Alla som är medlemmar i händelseprogrammet får ett sannolikhetsvärde mellan 0 och 100.

Vi sätter in sannolikhetsvärden i tre segment:

* Sannolikhet att registrera >50 % = segment med mycket sannolikhet
* Sannolikt att registrera >25 % till &lt;50 % = Sannolikt segment
* Sannolikhet för registrering &lt;25% = mindre sannolikhetssegment

När det är troligt att en person registrerar sig hamnar förutsägelsen i ett av dessa segment (alla som är medlemmar i ett program kommer att ingå i ett av dem). Om ett händelseprogram till exempel har 1000 medlemmar baserat på sannolikhetsprognoserna, kommer dessa 1000 att distribueras till segmenten _Mycket sannolikt_, _Sannolikt_ eller _Mindre sannolikt_ .

Därför har de som hamnar i segmentet Highly Troely större chans att anmäla sig till evenemanget.

Konvertering till register = # av personer i segment som är registrerade delat med # personer som faller in i segmentet (om till exempel 100 personer faller in i segmentet Mycket sannolikt och 60 av dem registrerar sig, är konverteringsgraden 60 %).

Konvertering % till register följer det här mönstret: Mycket sannolikt > Sannolikt > Mindre sannolikt.

**F: Hur använder jag insikterna?**

S: Bästa praxis innebär följande:

i. Du skapar ett program och sedan använder en Smart Campaign prediktiva filter med&quot;större än X&quot;, vilket skulle resultera i ett visst antal personer (till exempel 1 000) och ni kör kampanjen.

ii. Efter 24 timmar kan du på fliken [!UICONTROL Reports] se de planerade registreringarna som beräknas baserat på sannolikheten att registrera värden för alla personer som för närvarande är inbjudna.

iii. Om de planerade registreringarna är mindre än målet måste du bjuda in fler personer. Nu kan du se vilka insikter som visar vilket tröskelvärde som fungerade i tidigare program.

![Bild åtta](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Du kan skapa en ny smart kampanj med det tröskelvärdet för att bjuda in fler personer.

v. När som helst om du vill förstå varför ett projicerat tal visas kan du växla för att se målgruppsfördelningen mellan segment, deras konverteringsgrader från det förflutna och använda konverteringsgraden för den aktuella målgruppen (se skärmbilden nedan).

**F: Vad är segmenten efter registrering?**

S: Tre staplar, var och en representerar ett segment (Mycket sannolikt, Sannolikt, Mindre sannolikt).

**Lila prickad linje:** Genomsnittlig konverteringsgrad till registrering i det segmentet, baserat på tidigare liknande program.

**Blue bar:** Registreringsprocent för alla personer i det segmentet.

![Bild nio](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

Exempel: 100 personer har möjlighet att registrera > 50 % och 60 av dessa 100 personer. Mycket troligt har 60 % konvertering. Det innebär att alla medlemmar som läggs till i programmet är benägna att registrera värden, sedan läggs de in i segment och antalet registrerade personer i varje segmentkonverteringsgrad beräknas.

**F: Vad betyder &quot;Registered and Higher&quot;?**

S: Alla som är listade som registrerade eller som har en annan status med samma eller högre stegnummer.

Du kan skapa nya statusvärden för ett händelseprogram, men vi mappar dessa statusvärden med standardstatusvärden. Tänk på ett fall där en person flyttas från en inbjudan till en påminnelse, vilket är ett högre steg än registrering. Den här personen betraktas också som registrerad och visas i målspårningen.

![Bild tio](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**F: Hur beräknas planerade registreringar?**

S: Se nedan.

![Bild elva](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
