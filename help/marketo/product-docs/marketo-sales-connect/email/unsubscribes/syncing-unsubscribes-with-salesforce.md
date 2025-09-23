---
unique-page-id: 14746188
description: Synkronisera avbeställningar med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisera Avsluta prenumeration med Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 1%

---

# Synkroniserar Avbeställ med [!DNL Salesforce] {#syncing-unsubscribes-with-salesforce}

## Krav för att avbryta prenumerationen att synkronisera med [!DNL Salesforce] {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Synkronisering av avbruten prenumeration måste vara aktiverat (för nightly sync)
* Opt Out-fältet måste vara installerat i [!DNL Salesforce]
* Personposter i [!DNL Sales Connect] måste ha ett [!DNL Salesforce]-ID

**Push Unsubscribe**

När en avanmälan samlas in i [!DNL Sales Connect] skickar vi den till [!DNL Salesforce] i realtid och uppdaterar något av de avanmälningsfält som du har valt att synkronisera med. Om du har inaktiverat synkroniseringen av [!DNL Salesforce] kommer vi fortfarande att pusha över avanmälan till avanmälan via e-post.

**Avbeställ synkronisering**

När du har aktiverat synkroniseringen för att avbryta prenumerationen (steg 3 nedan) aktiveras synkroniseringen varje natt. Synkroniseringen sker en gång om dagen runt kl. 20 PST. :00 Det synkroniserar alla avbeställningar i Marketo Sales med fältet Avanmäl dig i Salesforce.

## Konfigurera Synkronisering för att avbryta prenumeration för [!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

Användare kan bestämma sig för om de vill synkronisera sin avanmälan med standardfältet för avanmälan via e-post som Marketo också kan synkronisera med, eller så kan de synkronisera med fältet för avanmälan från Marketo så att avanmälan från försäljning och avanmälan från marknadsföring kan differentieras.

1. Gå till [webbprogrammet](https://toutapp.com/login), klicka på kugghjulsikonen och välj **[!UICONTROL Settings]**.

   ![](assets/one-1.png)

1. Under [!UICONTROL Admin Settings] väljer du **[!UICONTROL Unsubscribes]**.

   ![](assets/two-2.png)

1. Klicka på **[!UICONTROL Syncing to Salesforce]** och aktivera sedan nattsynkroniseringen.

   ![](assets/three-2.png)

1. Markera fältet som du vill synkronisera till.

   ![](assets/4.png)

   | Fält | Beskrivning |
   |---|---|
   | **[!UICONTROL Sync to Salesforce Opt Out field]** | Markerat som standard uppdaterar bara fältet [!DNL Salesforce] avanmäl dig. |
   | **[!UICONTROL Sync to Marketo Sales Opt Out field]** | Om du vill avgränsa försäljning och marknadsföring väljer du det här alternativet för att uppdatera ytterligare [avanmälningsfält för Marketo.](#msoo) |

## Installera avanmälningsfältet i sidlayouten {#installing-the-opt-out-field-in-the-page-layout}

**Avanmäl dig via e-post**

E-postavanmälan är ett standardfält i [!DNL Salesforce] som kan installeras från [!DNL Salesforce]. Du måste vara en [!DNL Salesforce]-administratör för att kunna installera det.

1. Gå till [Salesforce.com](https://salesforce.com) och logga in.

   ![](assets/five-1.png)

1. Klicka på ditt användarnamn och välj **[!UICONTROL Setup]**.

   ![](assets/six-1.png)

1. I snabbsökningsrutan söker du efter antingen Kontakt eller Lead. I det här scenariot installerar vi fältet till kontaktsidans layout, men du vill installera för båda personposterna.

   ![](assets/seven-1.png)

1. Välj **[!UICONTROL Page Layouts]**.

   ![](assets/eight-1.png)

1. Välj **[!UICONTROL Edit]** bredvid sidlayouten som du vill lägga till fältet i.

   ![](assets/nine.png)

1. Välj **[!UICONTROL Fields]**.

   ![](assets/ten.png)

1. Dra och släpp [!UICONTROL Email Opt Out] i sidlayouten.

   ![](assets/11.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/twelve.png)

## Marketo Sales Opt Out {#marketo-sales-opt-out}

Fältet Marketo Sales Opt Out är ett anpassat fält som är tillgängligt för användare som har installerat Marketo [!DNL Sales Connect] Customizations.

När du har installerat Marketo [!DNL Sales Connect]-anpassningarna i [!DNL Salesforce] ser du fältet för avanmälan från Marketo.
