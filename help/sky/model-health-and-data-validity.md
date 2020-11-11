---
title: model-health-and-data-validity
description: Modellens hälsa och datavalidering
translation-type: tm+mt
source-git-commit: cd1b7e65c73de0b31f20289402f1c0832c382b33
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---


# Modellens hälsa och datavalidering

<br> 

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Så här bedömer du modellens hälsa.

Navigera till avsnittet [!UICONTROL **Modeller och Datahälsa**] under [!UICONTROL **Predictive Audiences**] under [!UICONTROL **Admin**] i Marketo Classic. Här ser du alla dina modeller och deras status.

![Bild ett](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som _bearbetas_ kan ta upp till 24 timmar att slutföra. Om det finns några _modeller som inte fungerar_ kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modellhälsa baserat på datainsamling och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/är fullständiga.
* **Datakvalitet**: Procentandel av attribut som innehåller bra, användbara data.
