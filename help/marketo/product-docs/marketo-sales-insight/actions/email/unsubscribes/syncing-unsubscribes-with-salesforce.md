---
description: Synkronisera avbeställningar med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisera avbeställningar med Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Synkronisera avbeställningar med Salesforce {#syncing-unsubscribes-with-salesforce}

Om du vill synkronisera avanmälan med ett avanmälningsfält i Salesforce kan du använda avanmälningssynkroniseringen i Salesforce.

## Krav för att avbryta prenumerationen på Synkronisera med Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Synkronisering av avbruten prenumeration måste vara aktiverat (för nightly sync)
* Fältet för avanmälan måste vara installerat i Salesforce
* Personposter i Marketo försäljning måste ha ett Salesforce-ID

**Push Unsubscribe**

När en avanmälan samlas in i Marketo Sales skickar vi den till Salesforce i realtid och uppdaterar något av avanmälningsfälten som du har valt att synkronisera med. Om du har inaktiverat Salesforce-synkroniseringen kommer vi fortfarande att pusha över avbeställningen till avanmälan via e-post.

**Avbeställ synkronisering**

När du har aktiverat synkroniseringen för att avbryta prenumerationen (steg 3 nedan) aktiveras synkroniseringen varje natt. Synkroniseringen sker en gång om dagen runt kl. 20.00 PST. Den synkroniserar alla avbeställningar i Marketo Sales med fältet Avanmäl dig i Salesforce.

>[!NOTE]
>
>Om du avbryter prenumerationen synkroniseras alla prenumerationer med Salesforce, men återprenumerationer synkroniseras inte. Om du vill ta bort en prenumeration från Marketo Sales och Salesforce avmarkerar du avprenumerationen i Salesforce och tar bort avprenumerationen i Marketo Sales.

## Konfigurera Synkronisera för att avbryta prenumeration för Salesforce {#configure-unsubscribe-sync-to-salesforce}

Användare kan bestämma sig för om de vill synkronisera sin avanmälan med standardfältet för avanmälan via e-post som Marketo också kan synkronisera med, eller så kan de synkronisera med fältet för avanmälan från Marketo så att avanmälan från försäljning och avanmälan från marknadsföring kan differentieras.

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Under Administratörsinställningar väljer du **Avbeställ**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Klicka på fliken **Integrationer**. Aktivera nattsynkronisering under Synkronisera med Salesforce.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Markera fältet som du vill synkronisera till.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Fält | Beskrivning |
   |---|---|
   | **Synkronisera med Salesforce-fältet för avanmälan** | Markerat som standard uppdaterar bara Salesforce-alternativfältet. |
   | **Synkronisera med fältet för avanmälan för Marketo-försäljning** | Om du vill avgränsa försäljning och marknadsföring väljer du det här alternativet för att uppdatera ytterligare [avanmälningsfält för Marketo.](#msoo) |

## Installera avanmälningsfältet i sidlayouten {#installing-the-opt-out-field-in-the-page-layout}

**Avanmäl dig via e-post**

Avanmäl dig via e-post är ett standardfält i Salesforce som kan installeras från Salesforce. Du måste vara Salesforce-administratör för att kunna installera det.

1. Gå till [Salesforce.com](https://salesforce.com) och logga in.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Klicka på ditt användarnamn och välj **Inställningar**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. I snabbsökningsrutan söker du efter antingen Kontakt eller Lead. I det här scenariot installerar vi fältet till kontaktsidans layout, men du vill installera för båda personposterna.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Välj **Sidlayouter**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Välj **Redigera** bredvid sidlayouten som du vill lägga till fältet i.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Välj **Fält**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Dra och släpp e-postavanmälan till sidlayouten.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Klicka på **Spara**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo Sales Opt Out {#marketo-sales-opt-out}

Fältet Marketo Sales Opt Out är ett anpassat fält som är tillgängligt för användare som har installerat Marketo Sales Insight-paketet [ från AppExchangen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

När du har installerat Marketo Sales Insight-paketet från AppExchangen till Salesforce visas fältet Marketo Sales Opt Out som är tillgängligt för dig.
