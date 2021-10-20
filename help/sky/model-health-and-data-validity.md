---
title: model-health-and-data-validity
description: Modellens hälsa och datavalidering
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
source-git-commit: 41a51afde7942d6973a01636810bc5862d023e99
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Modellens hälsa och datavalidering

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Se den viktigaste påverkande faktorn för var och en av dina sannolika AI-modeller. Se även de viktigaste faktorerna som leder till registrering av händelser, närvaro eller avanmälan.

>[!NOTE]
>
>Beteenden markerade med (+) påverkar prediktionerna positivt (och vice versa).

Så här bedömer du modellens hälsa.

Navigera till **[!UICONTROL Models and Data Health]** avsnitt under **[!UICONTROL Predictive Audiences]** i **[!UICONTROL Admin]** Marketo Classic. Här ser du alla dina modeller och deras status.

![Bild ett](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som _Bearbetar_ kan ta upp till 24 timmar att slutföra. För alla _Misslyckades_ modeller, kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modellhälsa baserat på datainsamling och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/är fullständiga.
* **Datakvalitet**: Procentandel av attribut som innehåller bra, användbara data.
