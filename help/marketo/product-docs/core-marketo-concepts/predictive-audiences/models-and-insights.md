---
description: Modeller och insikter - Marketo Docs - produktdokumentation
title: Modeller och insikter
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Modeller och insikter {#models-and-insights}

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Se den viktigaste påverkande faktorn för var och en av dina sannolika AI-modeller. Se även de viktigaste faktorerna som leder till registrering av händelser, närvaro eller avanmälan.

>[!NOTE]
>
>Beteenden markerade med (+) påverkar prediktionerna positivt (och vice versa).

Så här bedömer du modellens hälsa.

Navigera till **[!UICONTROL Models and Data Health]** avsnitt under **[!UICONTROL Predictive Audiences]** i **[!UICONTROL Admin]** Marketo Engage. Här ser du alla dina modeller och deras status.

![Bild ett](assets/models-and-insights-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som _Bearbetar_ kan ta upp till 24 timmar att slutföra. För alla _Misslyckades_ modeller, kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modellhälsa baserat på datainsamling och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/är fullständiga.
* **Datakvalitet**: Procentandel av attribut som innehåller bra, användbara data.
