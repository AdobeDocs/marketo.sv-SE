---
unique-page-id: 1147114
description: Anpassade fälttoken för programmedlem - Marketo Docs - produktdokumentation
title: Anpassade fälttoken för programmedlem
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Anpassade fälttoken för programmedlem {#program-member-custom-field-tokens}

## Token Support för anpassade programmedlemsfält {#token-support-for-program-member-custom-fields}

På baksidan av funktionerna för anpassade fält för programmedlemmar utökas stödet för anpassade fält för programmedlemmar i tokenramverk.

PMCF-token stöds under medlemsdomänen för tokens-familjen.

Medlemstoken används för fält som omfattas av programmedlemmens tillämpningsområde. I nuläget används medlemstoken även för att infoga unika värden från integrerade tjänstpartner. `{{member.webinar url}}`-token löser automatiskt personens unika bekräftelse-URL som genererats av tjänstprovidern. {{member.registration code}} matchar registreringskoden som tillhandahålls av tjänsteleverantören.

>[!NOTE]
>
>* Anpassade fält för programmedlemmar kan bara användas i ett program.
>* Det går inte att använda token för anpassade fält för programmedlemmar i: e-postförrubrik, datumtoken i väntesteg eller kodfragment.
>* Programmedlemmens status stöds inte i medlemstoken.

## Använda token för anpassade fält för programmedlemmar i Assets {#using-program-member-custom-field-tokens-in-assets}

Du kan infoga token för anpassade fält för programmedlemmar i e-postmeddelanden, landningssidor, SMS, push-meddelanden och webhooks.

**E-post**

1. Markera önskad e-postadress och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Klicka på ikonen Infoga token.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Sök efter och välj önskad token för anpassat fält för programmedlem, ange ett standardvärde och klicka på **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Glöm inte att godkänna e-postmeddelandet.

**Landningssidor**

1. Välj din landningssida och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >Designern för landningssidan öppnas i ett nytt fönster.

1. Dubbelklicka på textrutan där du vill lägga till variabeln.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Klicka där du vill att token ska vara och klicka sedan på ikonen Infoga token.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Sök efter och välj önskad token.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Ange ett standardvärde och klicka på **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Välj önskat SMS och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Klicka på knappen **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Sök efter och välj önskad token för anpassat fält för programmedlem. Ange en [!UICONTROL default value] och klicka på **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Klicka på listrutan SMS-åtgärder och välj **[!UICONTROL Approve & Close]**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Push-meddelanden**

1. Välj önskat push-meddelande och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Klicka på **[!UICONTROL Push Notification]**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Klicka på meddelandet i redigeraren och klicka på knappen `{{` för att hämta tokenväljaren.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Sök efter och välj önskad token för anpassat fält för programmedlem. Ange ett standardvärde och klicka på **[!UICONTROL Insert]**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Klicka på **[!UICONTROL Finish]** för att spara och avsluta (eller **[!UICONTROL Next]** för att granska först).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Om det anpassade fältet Programmedlem för en medlem i programmet inte har något värde ersätts variabeln med standardvärdet om det har angetts.

## Använda token för anpassade fält för programmedlemmar i kampanjer {#using-program-member-custom-field-tokens-in-campaigns}

Anpassade fälttoken för programmedlem kan användas i:

* Skapa uppgift
* Skapa uppgift i Microsoft
* Intressanta ögonblick
* Ändra flödesåtgärder för datavärde
* Webhooks
