---
unique-page-id: 2949962
description: Växla synlighet för ett formulärfält dynamiskt - Marketo Docs - produktdokumentation
title: Växla synlighet för ett formulärfält dynamiskt
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Växla synlighet för ett formulärfält dynamiskt {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Lägg till en landsväljarlista i ditt formulär](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

En bra egenskap hos Marketo-formulär är att du dynamiskt kan dölja/visa formulärfält eller [fältuppsättningar](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exempel**
>
>I det här exemplet döljer vi fältet **Delstat** såvida inte **Land** har valts som &quot;USA&quot;.

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-8.png)

1. Markera formuläret och klicka på **[!UICONTROL Edit Form]**.

   ![](assets/editform-1.png)

1. Markera fältet som du vill visa/dölja dynamiskt och klicka på länken för **[!UICONTROL Visibility Rules]**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Sök efter och markera det fält som du vill skapa ett villkor runt.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Markera operatorn.

   >[!TIP]
   >
   >Det här är coolt eftersom du kan välja oskarpa matchningar som [!UICONTROL starts with].

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Markera de värden du vill söka efter och klicka sedan utanför listrutan.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Du kan markera flera värden genom att klicka på dem när listrutan är öppen. Du kan till exempel välja USA och Kanada.

   >[!NOTE]
   >
   >Vi konverterade tidigare Land till en fälttyp för plocklista och [lade till alla länder som värden](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Och det är allt! När man fyller i blanketten och väljer USA som land visas fältet State dynamiskt med de alternativ som anges.

>[!IMPORTANT]
>
>Formulärfältets beteende fungerar sömlöst när fältvärden anges/uppdateras via anpassade skript med [API-funktioner](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} i Forms 2.0.
>
>Villkorliga fält kanske inte fungerar som förväntat om fältvärdena ändras av andra externa skript än Forms 2.0 JavaScript API.
