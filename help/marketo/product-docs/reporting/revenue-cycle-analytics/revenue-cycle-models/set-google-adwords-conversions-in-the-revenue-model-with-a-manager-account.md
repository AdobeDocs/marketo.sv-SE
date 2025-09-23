---
unique-page-id: 7504923
description: Ange  [!DNL Google AdWords] konverteringar i intäktsmodellen med ett Manager-konto - Marketo Docs - produktdokumentation
title: Ange  [!DNL Google AdWords] konverteringar i intäktsmodellen med ett hanterarkonto
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Ange [!DNL Google AdWords]-konverteringar i intäktsmodellen med ett hanterarkonto {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Länka ditt [!DNL Google AdWords]-konto till Marketo för att automatiskt överföra offlinekonverteringsdata från Marketo till [!DNL Google AdWords]. Från gränssnittet [!DNL AdWords] kan du sedan enkelt se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg du vill spåra) efter att du [lagt till anpassade kolumner](https://support.google.com/adwords/answer/3073556) i [!DNL AdWords].

Om du har flera [!DNL Google Adwords]-konton kan du använda ett [[!DNL Google AdWords] hanterarkonto](https://www.google.com/adwords/manager-accounts/) (tidigare kallat Mitt klientcenter) för att integrera dem med Marketo.

Du kan mappa [!DNL AdWords] offlinekonverteringar till en eller flera steg i en intäktsmodell. Det finns två sätt:

* Scenåtgärd
* [!DNL AdWords]-mappning

>[!PREREQUISITES]
>
>[Lägg till [!DNL Google AdWords] som en startpunktstjänst med ett hanterarkonto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Använd scenåtgärd {#use-stage-action}

Mappa en [!DNL AdWords]-konvertering under Stage Actions.

1. Välj det steg som du vill mappa till en [!DNL AdWords]-konvertering.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Välj **[!UICONTROL Stage Actions]** i listrutan **[!UICONTROL Set AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Ange en **[!DNL AdWords]-konvertering**.

   >[!NOTE]
   >
   >En annan [!DNL AdWords]-konvertering kan väljas för varje underordnat konto.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Tips! Om du inte har några [!DNL AdWords]-konverteringar skapar du en genom att klicka på **[!UICONTROL +New Conversion]**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. När du har mappat alla dina [!DNL AdWords]-konverteringar till intäktsfaser går du tillbaka till sammanfattningssidan. Markera **[!UICONTROL Model Actions]** och välj **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Proffstips: Lägg till en ny konvertering {#pro-tip-add-a-new-conversion}

Proffstips! En ny offlinekonvertering för [!DNL AdWords] kan skapas från Marketo.

>[!CAUTION]
>
>Nya konverteringar som skapats från Marketo har &quot;optimeringsinställningen&quot; aktiverad. Det innebär att [!DNL AdWords] anbudsstrategier tillåts optimera dina bud för dessa konverteringar. Du kan ändra den här inställningen från ditt [!DNL AdWords]-konto.

1. Välj **[!UICONTROL Stage Actions]** i listrutan **[!UICONTROL Set AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Välj **[!UICONTROL New Conversion]**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Ange ett **konverteringsnamn**. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Underbar! Den nya konverteringen visas i ditt [!DNL AdWords]-konto.

## Använd [!DNL AdWords]-mappning {#use-adwords-mapping}

Du kan associera alla dina modellfaser med din [!DNL AdWords]-konvertering på ett ställe med [!DNL AdWords]-mappningar.

1. Välj **[!UICONTROL Edit AdWords Mappings]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Välj önskat **[!DNL AdWords]-konto** och önskad **[!DNL AdWords]konvertering** för varje fas som du vill spåra.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. När du har mappat dina faser klickar du på **[!UICONTROL Save]**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. När du har mappat alla dina [!DNL AdWords]-konverteringar till intäktsfaser går du tillbaka till sammanfattningssidan. Markera **[!UICONTROL Model Actions]** och välj **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Om du vill visa offlinekonverteringsdata måste du logga in på ditt [!DNL AdWords]-konto. Vi rekommenderar att du använder deras [anpassade kolumnfunktion](https://support.google.com/adwords/answer/3073556) för att skapa konverteringskolumner för varje offlinekonvertering som du importerar från Marketo.
