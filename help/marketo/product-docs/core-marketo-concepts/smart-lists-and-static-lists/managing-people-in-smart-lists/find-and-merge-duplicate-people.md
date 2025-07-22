---
unique-page-id: 557339
description: Sök och sammanfoga duplicerade personer - Marketo Docs - produktdokumentation
title: Sök och sammanfoga duplicerade personer
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Sök och sammanfoga duplicerade personer {#find-and-merge-duplicate-people}

Marketo Engage deduplicerar automatiskt när nya personer kommer in i systemet. CRM-data kan dock ha skickats över dubbletter från början. Så här sammanfogar du dem.

>[!CAUTION]
>
>Att sammanfoga personer är permanent, det finns inget ångra-alternativ.

>[!PREREQUISITES]
>
>Om du söker efter och sammanfogar dubbletter används [inbyggda/systemsmarta listor](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo avduplicerar inte automatiskt mot en [!DNL Salesforce]- eller [!DNL Microsoft Dynamics]-synkronisering eller när du anger personer manuellt.

## Sök dubbletter {#find-duplicates}

1. Gå till området **[!UICONTROL Database]**.

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >Det går kanske inte att sammanfoga personer i Marketo om du använder ett [!DNL Salesforce]-personkonto. Sammanfoga posterna i [!DNL Salesforce] om det är möjligt.

1. Välj den smarta listan för **[!UICONTROL Possible Duplicates]** och klicka på fliken **[!UICONTROL People]**.

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >Du kan också [söka efter dubbletter av personer med anpassad logik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## Sammanfoga personer manuellt {#merge-people-manually}

>[!CAUTION]
>
>När du sammanfogar personer och den person som förlorar har ett anpassat Marketo-objekt, kopplas det _inte_ till den vinnande personen. Överför det anpassade objektet på nytt innan du utför sammanfogningen.

1. Markera dubbletterna genom att hålla ned Ctrl/Cmd och klicka på **[!UICONTROL Merge People]**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Du kan ha två eller flera dubbletter för samma person - markera alla samtidigt.

1. Du kommer att se värdena mellan posterna som _inte_ matchar. Välj det värde som du vill behålla för varje fält. Klicka på **[!UICONTROL Merge]** när du är klar. Om du inte vill ha något av värdena kan du kontrollera **[!UICONTROL Custom]** och ange ett värde.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >När man sammanfogar personer manuellt blir den första personen&quot;vinnaren&quot;. Så om du sammanfogar post-ID:n 198 och 1999 på fliken Folk och klickar på 199 först blir 199 post-ID:t för de sammanfogade personerna. Detta gäller även om fler än två poster sammanfogas.

   >[!TIP]
   >
   >Det är bättre att sammanfoga än att ta bort. Du sparar all historik (sidbesök, länkklick, e-postöppningar, formulärfyllningar osv.).

## Effekt i Salesforce {#effect-in-salesforce}

Om du har Salesforce-integrering finns det några noteringar om effekten av att sammanfoga leads i Salesforce.

* När endast Leads eller endast Kontakter sammanfogas, sammanfogas de enligt normala [!DNL Salesforce]-regler.
* När du sammanfogar leads och kontakter konverteras alla leads till kontakter innan de sammanfogas enligt de normala [!DNL Salesforce]-reglerna.

Mer information om Salesforce beteende när du sammanfogar leads eller kontakter finns i följande [!DNL Salesforce]-dokument:

* [Sammanfogar dubblettrader](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&language=en_US){target="_blank"}
* [Sammanfogar dubblettkontakter](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&language=en_US){target="_blank"}

## Masssammanslagning {#bulk-merging}

Om du har för många dubbletter för att slå samman manuellt kontaktar du Adobe Account Team (din kontoansvarige) för att diskutera dina alternativ.
