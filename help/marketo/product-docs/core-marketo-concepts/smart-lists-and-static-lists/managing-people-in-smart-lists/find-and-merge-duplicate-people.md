---
unique-page-id: 557339
description: Sök och sammanfoga duplicerade personer - Marketo Docs - produktdokumentation
title: Sök och sammanfoga duplicerade personer
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Sök och sammanfoga duplicerade personer {#find-and-merge-duplicate-people}

Marketo Engage tar automatiskt bort dubbletter när nya personer kommer in i systemet. CRM-data kan dock ha skickats över dubbletter från början. Så här sammanfogar du dem.

>[!CAUTION]
>
>Att sammanfoga personer är permanent, det finns inget ångra-alternativ.

>[!PREREQUISITES]
>
>Att söka efter och sammanfoga dubbletter innebär att [inbyggda/systemsmarta listor](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo avlastar inte automatiskt från en Salesforce- eller Microsoft Dynamics-synkronisering, och inte heller när du anger personer manuellt.

## Sök dubbletter {#find-duplicates}

1. Gå till **[!UICONTROL Database]** område.

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >Det kanske inte fungerar att sammanfoga personer i Marketo om du använder ett Salesforce-personkonto. Sammanfoga posterna i Salesforce om det är möjligt.

1. Välj **[!UICONTROL Possible Duplicates]** System Smart List och klicka på **[!UICONTROL People]** -fliken.

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >Du kan också [Sök efter duplicerade personer med anpassad logik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## Sammanfoga personer manuellt {#merge-people-manually}

>[!CAUTION]
>
>När du sammanfogar personer och den person som förlorar har ett anpassat Marketo-objekt, kommer det att _not_ och associeras med den vinnande personen. Överför det anpassade objektet på nytt innan du utför sammanfogningen.

1. Markera dubbletterna genom att hålla ned Ctrl/Cmd och klicka och sedan på **[!UICONTROL Merge People]**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Du kan ha två eller flera dubbletter för samma person - markera alla samtidigt.

1. Du ser värdena mellan posterna som _inte_ matcha. Välj det värde som du vill behålla för varje fält. Klicka **[!UICONTROL Merge]** när det är klart. Om du inte vill ha något av värdena kan du kontrollera **[!UICONTROL Custom]** och ange ett värde.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >När man sammanfogar personer manuellt blir den första personen&quot;vinnaren&quot;. Så om du sammanfogar post-ID:n 198 och 1999 på fliken Folk och klickar på 199 först blir 199 post-ID:t för de sammanfogade personerna. Detta gäller även om fler än två poster sammanfogas.

   >[!TIP]
   >
   >Det är bättre att sammanfoga än att ta bort. Du sparar all historik (sidbesök, länkklick, e-postöppningar, formulärfyllningar osv.).

## Effekt i Salesforce {#effect-in-salesforce}

Om du har Salesforce-integrering finns det några noteringar om effekten av att sammanfoga leads i Salesforce.

* När du bara sammanfogar leads eller enbart kontakter sammanfogas de enligt vanliga Salesforce-regler.
* När du sammanfogar Leads och Kontakter konverteras alla Leads till Kontakter innan de sammanfogas enligt vanliga Salesforce-regler.

Mer information om Salesforce-beteendet när du sammanfogar leads eller kontakter finns i följande Salesforce-dokument:

* [Sammanfoga dubblettrader](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US){target="_blank"}
* [Sammanfoga dubblettkontakter](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US){target="_blank"}

## Masssammanslagning {#bulk-merging}

Om du har för många dubbletter för att sammanfoga manuellt kontaktar du kontogruppen (din kontohanterare) på Adobe för att diskutera dina alternativ.
