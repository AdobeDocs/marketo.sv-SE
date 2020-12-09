---
unique-page-id: 6095029
description: Ange Google AdWords-konverteringar i intäktsmodellen - Marketo Docs - Produktdokumentation
title: Ange Google AdWords-konverteringar i intäktsmodellen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# Ange Google AdWords-konverteringar i intäktsmodellen {#set-google-adwords-conversions-in-the-revenue-model}

Länka ditt Google AdWords-konto till Marketo för att automatiskt överföra konverteringsdata offline från Marketo till Google AdWords. Sedan kan ni från gränssnittet för AdWords enkelt se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg ni vill spåra) efter att ni har [lagt till anpassade kolumner](https://support.google.com/adwords/answer/3073556) i AdWords.

>[!NOTE]
>
>Det här är en push-integrering från Marketo till Google AdWords. Konverteringsdata visas *bara* i Google AdWords-portalen**, inte i Marketo-gränssnittet. **

Läs mer om [Googles importfunktion](https://support.google.com/adwords/answer/2998031?hl=en)för offlinekonvertering.  Mappa AdWords-offlinekonverteringar till en eller flera steg i en intäktsmodell. Det finns tre sätt att mappa:

* Konvertering av ord
* Scenåtgärd
* AdWords-mappning

Du kan skapa en ny offlinekonvertering för AdWords från Marketo om du använder Stage Action.

>[!PREREQUISITES]
>
>* [Lägg till Google AdWords som en LaunchPoint-tjänst](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

>



## Använd AdWords-konvertering {#use-adwords-conversion}

1. Gå till **Analytics** .

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Välj en modell.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Klicka på **Redigera utkast**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Välj det intäktsstadium som du vill mappa till en AdWords-konvertering.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Välj den **AdWords Conversion** som du vill mappa till Marketo-scenen.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Snyggt! Dina konverteringsdata för AdWords kommer att överföras till dina Google AdWords vid den surfplats du valt.

## Använd scenåtgärd {#use-stage-action}

Du kan också mappa en AdWords-konvertering under Stage-åtgärder.

1. Välj det steg som du vill mappa till en AdWords-konvertering.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Under listrutan **Scenåtgärder** väljer du **Ställ in radkonvertering**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Välj en **AdWords-konvertering**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Tips**: Om du inte har några AdWords-konverteringar skapar du en genom att klicka på **+Ny konvertering**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Klicka på **Spara**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. När du är klar med att mappa alla dina AdWords-konverteringar till intäktsfaser går du tillbaka till sammanfattningssidan. Välj **Modellåtgärder** och välj **Godkänn steg**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Proffstips: Lägg till en ny konvertering {#pro-tip-add-a-new-conversion}

Proffstips! En ny offlinekonvertering för AdWords kan skapas från Marketo.

>[!CAUTION]
>
>Nya konverteringar som skapats från Marketo har optimeringsinställningen aktiverad. Det innebär att AdWords anbudsstrategier kan optimera dina bud för dessa konverteringar. Du kan ändra den här inställningen från ditt AdWords-konto.

1. Under listrutan **Scenåtgärder** väljer du **Ställ in radkonvertering**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Välj **Ny konvertering**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Ange ett **konverteringsnamn**. Klicka på **Spara**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Underbar! Den nya konverteringen visas i ditt AdWords-konto.

## Använd AdWords-mappning {#use-adwords-mapping}

Du kan koppla alla dina modellfaser till din AdWords-konvertering på ett och samma ställe med hjälp av AdWords Mappings.

1. Välj **Redigera AdWords-mappningar**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Välj önskad **AdWords-konvertering** för varje scen som du vill spåra.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. När du har mappat dina faser klickar du på **Spara**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. När du är klar med att mappa alla dina AdWords-konverteringar till intäktsfaser går du tillbaka till sammanfattningssidan. Välj **Modellåtgärder** och välj **Godkänn steg**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Om du vill visa offlinekonverteringsdata måste du logga in på ditt AdWords-konto. Vi rekommenderar att du använder deras [anpassade kolumnfunktion](https://support.google.com/adwords/answer/3073556) för att skapa konverteringskolumner för varje offlinekonvertering som du importerar från Marketo.
