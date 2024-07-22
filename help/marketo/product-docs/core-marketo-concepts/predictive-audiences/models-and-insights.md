---
description: Modeller och insikter - Marketo Docs - produktdokumentation
title: Modeller och insikter
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 86f9e9f13b24a82deb50ec4c398035d7d7479d20
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Modeller och insikter {#models-and-insights}

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Se den viktigaste påverkande faktorn för var och en av dina sannolika AI-modeller. Se även de viktigaste faktorerna som leder till registrering av händelser, närvaro eller avanmälan.

>[!NOTE]
>
>Beteenden markerade med (+) påverkar prediktionerna positivt (och vice versa).

Så här bedömer du modellens hälsa.

Navigera till avsnittet **[!UICONTROL Models and Data Health]** under **[!UICONTROL Predictive Audiences]** i området **[!UICONTROL Admin]** i Marketo Engage. Här ser du alla dina modeller och deras status.

![Bild ett](assets/models-and-insights-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som är _Bearbetar_ kan ta upp till 24 timmar att slutföra. Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"} för alla _Misslyckade_-modeller.
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modellhälsa baserat på datainsamling och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/har slutförts.
* **Datakvalitet**: Procentandel attribut som innehåller bra, användbara data.
