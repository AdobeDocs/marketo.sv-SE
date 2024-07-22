---
description: Förväntat beteende - Marketo Docs - produktdokumentation
title: Förväntat beteende
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: fb77478cdcd2b455e9f2359e16aca50143ce492c
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Förväntat beteende {#expected-behavior}

I den här artikeln hittar du information om förväntat beteende som är kopplat till Predictive Audiences (PA).

## Funderna om data och integritet

* All nödvändig databehandling för AI/ML-modellerna äger rum i Nordamerika.
* AI/ML-modeller använder inte specifik ledinformation som för- eller efternamn, kön, e-post, kontaktnummer osv. Modeller använder bara allmänna attribut som härletts från firmgrafik och aktivitetsloggar.

**För prediktiva målgrupper kan du förvänta dig följande beteende**

* PA är tillgängligt både i Marketo Skyn och i Marketo Classic. Följande specifika funktioner är tillgängliga:
   * Prediktiva filter - [!DNL Sky/Classic]
   * Planerade registreringar - [!DNL Sky/Classic]
   * Sannolikhetsprognoser på huvudnivå - [!DNL Sky/Classic]
   * Mål och spårning - endast [!DNL Sky]
   * Insikter och rekommendationer - endast [!DNL Sky]
* Den första aktiveringen tar **24-48 timmar** för alla processer att slutföras när PA har aktiverats. Du kommer att se alla funktioner för prediktiva målgrupper och prediktiva filter i gränssnittet, men det kan ta upp till 24 timmar innan de här funktionerna börjar fungera.
* **Förutsättningar genereras bara för nya kampanjer som skapas efter att funktionen har aktiverats.**

**Det finns ytterligare saker att tänka på när det gäller prediktiva filter**:

* Filtren Registrering och Närvaro kan bara användas med event- eller webbinariprogram. Filtren Lookalike och Unsubscribe kan användas i e-post-, event- och webbinariprogram.
* Du kan använda prediktiva filter på en smart kampanj även om det överordnade programmet skapas innan prediktiva filter aktiveras.
* Prediktiva filter är inte tillgängliga för utlösarkampanjer.
* Om du vill köra en smart kampanj måste troliga filter användas tillsammans med andra vanliga filter.
* Funktionen Sparade regler kan inte användas i kampanjer som innehåller prediktiva filter.
* Du kan använda **upp till 5** prediktiva filter i en smart lista.
* Prediktiva filter kan behandla **maximalt 1 miljon kvalificerade leads**.
* Du kan ha **upp till 50 aktiva program** med prediktiva filter. Ett aktivt program är ett program som använder prediktiva filter och har schemalagts minst en gång.

## När är inte projicerade registreringar tillgängliga?

Projicerade registreringar är inte tillgängliga i följande fall:

* om programmet skapades innan prediktiva målgrupper lades till
* när programstatus inte är mappad till systemstatus
* när det inte finns några medlemmar i programmet
* om det inte finns några tidigare liknande program under de senaste sex månaderna som uppfyller de obligatoriska kriterierna
