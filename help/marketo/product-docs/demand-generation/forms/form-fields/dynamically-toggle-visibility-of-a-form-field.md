---
unique-page-id: 2949962
description: Växla synlighet för ett formulärfält dynamiskt - Marketo Docs - Produktdokumentation
title: Växla synlighet för ett formulärfält dynamiskt
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---


# Växla synlighet för ett formulärfält dynamiskt {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Lägg till en landsväljare i formuläret](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



En bra egenskap hos Marketo-formulär är att du dynamiskt kan dölja/visa formulärfält eller [fältuppsättningar](add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exempel**
>
>I det här exemplet döljer vi fältet **Delstat** såvida inte **Land** har valts som &quot;USA&quot;.

1. Gå till **Marknadsföringsaktiviteter** och **aktiviteter**.

   ![](assets/login-marketing-activities-8.png)

1. Markera formuläret och klicka på **Redigera** **formulär**.

   ![](assets/editform-1.png)

1. Markera det fält som du vill visa/dölja dynamiskt och klicka på länken för **Synlighetsregler** ****.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Sök efter och markera det fält som du vill skapa ett villkor runt.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Markera operatorn.

   >[!TIP]
   >
   >Det här är coolt eftersom du kan välja oskarpa matchningar som &quot;börjar med&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Markera de värden du vill söka efter och klicka sedan utanför listrutan.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Du kan markera flera värden genom att klicka på dem när listrutan är öppen. Du kan till exempel välja USA och Kanada.

   >[!NOTE]
   >
   >Vi har tidigare konverterat Land till fälttyp för plocklista och [lagt till alla länder som värden](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Klicka på **Spara**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Och det är allt! När man fyller i blanketten och väljer USA som land visas fältet State dynamiskt med de alternativ som anges.

>[!NOTE]
>
>**Djupdykning**
>
>Vill du veta mer om [formulär](http://docs.marketo.com/display/docs/forms)?

