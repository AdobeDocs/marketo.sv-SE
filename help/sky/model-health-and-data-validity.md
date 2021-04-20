---
title: model-health-and-data-validity
description: Modellens hälsa och datavalidering
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Modellens hälsa och datavalidering

<br> 

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Så här bedömer du modellens hälsa.

Navigera till avsnittet **[!UICONTROL Models and Data Health]** under **[!UICONTROL Predictive Audiences]** i **[!UICONTROL Admin]**-området i Marketo Classic. Här ser du alla dina modeller och deras status.

![Bild ett](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som är _Bearbetning_ kan ta upp till 24 timmar att slutföra. För alla _misslyckade_-modeller kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modellhälsa baserat på datainsamling och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/är fullständiga.
* **Datakvalitet**: Procentandel av attribut som innehåller bra, användbara data.
