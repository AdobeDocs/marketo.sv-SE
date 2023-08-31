---
description: Prediktiva filter - Marketo Docs - produktdokumentation
title: Prediktiva filter
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
source-git-commit: 9019cb4b81fb3acd744e644d51059644af454e5e
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Prediktiva filter {#predictive-filters}

Som en del av Predictive Audiences erbjuder Marketo en grupp AI/ML-baserade filter i smarta listor inom smarta kampanjer.

![Bild ett](assets/predictive-filters-1.png)

>[!NOTE]
>
>Filtren&quot;Sannolikt att delta&quot; och&quot;Sannolikt att registrera&quot; kan bara användas i händelse- eller e-postprogram. &quot;Sannolikhet för att säga upp prenumerationen&quot;, &quot;Lookalike of Program Members&quot; och &quot;Lookalike of Smart List Members&quot; kan användas i alla programtyper.

## Sannolikhet att delta {#likelihood-to-attend}

Det här filtret används för att effektivt begränsa er målgrupp. Detta hjälper er att rikta in och bjuda in leads som har större sannolikhet att **deltar** ditt webbinarium eller event. Observera att&quot;Sannolikhet att delta&quot; kommer att vara ditt nuvarande eventprogram.

![Bild två](assets/predictive-filters-2.png)

## Sannolikhet för registrering {#likelihood-to-register}

Liknar _Sannolikhet att delta_ filtrera, använd det här filtret för att begränsa målgrupper och målleads som har större sannolikhet att **registrerar** för webbinariet eller evenemanget.

![Bild tre](assets/predictive-filters-3.png)

## Sannolikhet för avbeställning {#likelihood-to-unsubscribe}

Detta filtrerar publiken efter om de har en hög eller låg sannolikhet för att sluta prenumerera under de kommande två veckorna. Du kan använda detta för att rikta in dig på utmattning på olika sätt och mer effektivt. Tröskelvärdet för att avbryta prenumerationen är dynamiskt och styrs av en AI-modell som tar hänsyn till flera attribut, inklusive ledtid i databasen och lead-aktiviteter.

![Bild fyra](assets/predictive-filters-4.png)

>[!NOTE]
>
>Sannolikheten för att delta/registrera/avbryta prenumeration-filter måste användas tillsammans med andra standardfilter.

## Lookalike of Program Members/Lookalike of Smart List Members {#lookalike-of-members}

Dessa två filter hjälper er att utöka er nuvarande målgrupp genom att rikta in er på fler leads som liknar medlemmar i andra program eller Smart List. Filtren Lookalike tar hänsyn till fler än 50 faktorer, inklusive leadattribut, e-postaktivitet, webbaktivitet och engagemang.

Klicka **[!UICONTROL Add Constraint]** om du vill välja villkor för att medlemmarna i de valda programmen ska lyckas.

Klicka på **+** om du enkelt vill lägga till flera program/smarta listor till ett filter.

![Bild fem](assets/predictive-filters-5.png)

## Saker att notera {#things-to-note}

* Du kan använda prediktiva filter på en smart kampanj även om det överordnade programmet skapas innan prediktiva filter aktiveras.
* Prediktiva filter är inte tillgängliga för utlösarkampanjer.
* Kloning eller rörliga kampanjer som innehåller prediktiva filter stöds inte.
* Du kan använda upp till 5 prediktiva filter i en smart lista.
* Om Marketo Engage påträffar ett fel vid utvärderingen av prediktiva filter avbryts kampanjkörningen automatiskt och du får ett meddelande i Marketo meddelandecenter.
* Prediktiva filter har för närvarande en indatagräns på 1 miljon kvalificerade personer.
* Du kan ha upp till 50 aktiva program med prediktiva filter.
