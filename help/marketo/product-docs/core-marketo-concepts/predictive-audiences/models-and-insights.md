---
description: Modeller och insikter - Marketo Docs - produktdokumentation
title: Modeller och insikter
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Modeller och insikter {#models-and-insights}

Modellernas prestanda beror på kvaliteten och fullständigheten hos indata. Se den viktigaste påverkande faktorn för var och en av dina sannolika AI-modeller. Se även de viktigaste faktorerna som leder till snabbare/lägre registrering, närvaro vid händelse eller avanmälan.

>[!NOTE]
>
>Beteenden markerade med (+) påverkar prediktionerna positivt (och vice versa).

Så här bedömer du din modells hälsa.

Navigera till avsnittet **[!UICONTROL Models and Data Health]** under **[!UICONTROL Predictive Audiences]** i området **[!UICONTROL Admin]** i Marketo Engage. Här ser du alla dina modeller och deras status.

![Bild ett](assets/models-and-insights-1.png)

* **Utbildningsstatus**: Anger om din modell aktivt tränar (förbättrar prognoser). Kursen sker automatiskt varannan vecka. Alla modeller som är _Bearbetar_ kan ta upp till 24 timmar att slutföra. Kontakta _Marketo Support_ för alla [Misslyckade](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}-modeller.
* **Bedömningsstatus**: Anger om din modell aktivt beräknar prognoser (sannolikhetsprocent) för programmedlemmar.
* **Prestanda**: Kategorisering av din modells hälsa baserat på datakvalitet och datakvalitet (se nedan).
* **Datakompatibilitet**: Procentandel av dataattribut som finns/har slutförts.
* **Datakvalitet**: Procentandel attribut som innehåller bra, användbara data.
* **Senaste utbildning**: Datumet för den modell som är bäst av utvärderingen mellan den aktuella modellen och den nya modellen som har tränats varannan vecka.
