---
title: model-health-and-data-validity
description: Modellens hälsa och datavalidering
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# Modellens hälsa och datavalidering

<br> 

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Så här bedömer du modellens hälsa.

Navigera till avsnittet **[!UICONTROL Models and Data Health]** under **[!UICONTROL Predictive Audiences]** i området **[!UICONTROL Admin]** i Marketo Classic. Här ser du alla dina modeller och deras status.

![Bild ett](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som är _Bearbetning_ kan ta upp till 24 timmar att slutföra. För alla _misslyckade_-modeller kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modellhälsa baserat på datainsamling och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/är fullständiga.
* **Datakvalitet**: Procentandel av attribut som innehåller bra, användbara data.
