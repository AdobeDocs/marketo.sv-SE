---
description: Synkronisera avbeställningar med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisera Avsluta prenumeration med Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Synkroniserar Avbeställ med [!DNL Salesforce] {#syncing-unsubscribes-with-salesforce}

Om du vill synkronisera avanmälan med ett avanmälningsfält i Salesforce kan du använda Salesforce avanmälningssynkronisering.

## Krav för att avbryta prenumerationen på Synkronisera med Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Synkronisering av avbruten prenumeration måste vara aktiverat (för nightly sync)
* Opt Out-fältet måste vara installerat i [!DNL Salesforce]
* Personposter i [!DNL Marketo Sales] måste ha ett [!DNL Salesforce]-ID

**Push Unsubscribe**

När en avanmälan samlas in i [!DNL Marketo Sales] skickar vi den till [!DNL Salesforce] i realtid och uppdaterar något av de avanmälningsfält som du har valt att synkronisera med. Om du har inaktiverat synkroniseringen av [!DNL Salesforce] kommer vi fortfarande att pusha över avanmälan till avanmälan via e-post.

**Avbeställ synkronisering**

När du har aktiverat synkroniseringen för att avbryta prenumerationen (steg 3 nedan) aktiveras synkroniseringen varje natt. Synkroniseringen sker en gång om dagen runt kl. 20 PST. :00 Det synkroniserar alla avbeställningar i Marketo Sales med fältet Avanmäl dig i Salesforce.

>[!NOTE]
>
>Synkronisering av avanmälan med Salesforce kommer att synkronisera avanmälan, men det kommer inte att synkronisera återprenumerationer. Om du inte längre vill prenumerera på Marketo Sales och Salesforce avmarkerar du avbeställningen i Salesforce och tar bort avbeställningen i Marketo Sales.

## Konfigurera Synkronisering för att avbryta prenumeration för [!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

Användare kan bestämma sig för om de vill synkronisera sin avanmälan med standardfältet för e-postavanmälan som Marketo också kan synkronisera med, eller så kan de synkronisera med fältet [!DNL Marketo Sales] avanmäl dig så att avanmälan av försäljning och avanmälan av marknadsföring kan differentieras.

1. Klicka på kugghjulsikonen och välj **[!UICONTROL Settings]**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Under [!UICONTROL Admin Settings] väljer du **[!UICONTROL Unsubscribes]**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Klicka på fliken **[!UICONTROL Integrations]**. Aktivera nattsynkronisering under [!UICONTROL Sync to Salesforce].

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Markera fältet som du vill synkronisera till.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Fält | Beskrivning |
   |---|---|
   | **Synkronisera med fältet [!DNL Salesforce] Avanmäl dig** | Markerat som standard uppdaterar bara fältet [!DNL Salesforce] avanmäl dig. |
   | **Synkronisera med fältet [!DNL Marketo Sales] Avanmäl dig** | Om du vill avgränsa försäljning och marknadsföring väljer du det här alternativet för att uppdatera ytterligare [[!DNL Marketo Sales] avanmälningsfält.](#msoo) |

## Installera avanmälningsfältet i sidlayouten {#installing-the-opt-out-field-in-the-page-layout}

**Avanmäl dig via e-post**

E-postavanmälan är ett standardfält i [!DNL Salesforce] som kan installeras från [!DNL Salesforce]. Du måste vara en [!DNL Salesforce]-administratör för att kunna installera det.

1. Gå till [Salesforce.com](https://salesforce.com) och logga in.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Klicka på ditt användarnamn och välj **[!UICONTROL Setup]**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. I snabbsökningsrutan söker du efter antingen Kontakt eller Lead. I det här scenariot installerar vi fältet till kontaktsidans layout, men du vill installera för båda personposterna.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Välj **[!UICONTROL Page Layouts]**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Välj **[!UICONTROL Edit]** bredvid sidlayouten som du vill lägga till fältet i.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Välj **[!UICONTROL Fields]**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Dra och släpp [!UICONTROL Email Opt Out] i sidlayouten.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo Sales Opt Out {#marketo-sales-opt-out}

Fältet Marketo Sales Opt Out är ett anpassat fält som är tillgängligt för användare som har installerat Marketo Sales Insight-paketet [ från AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

När du har installerat Marketo Sales Insight-paketet från AppExchange till Salesforce ser du Marketo avanmälningsfält.
