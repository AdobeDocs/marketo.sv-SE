---
unique-page-id: 4720232
description: Skapa en ny kontolista - Marketo Docs - produktdokumentation
title: Skapa en ny kontolista
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Skapa en ny kontolista {#create-a-new-account-list}

Skapa och överför en lista över organisations- och domännamn för att rikta in dessa nyckelkonton mot personaliserade kampanjer.

>[!NOTE]
>
>Den här artikeln gäller endast äldre kunder med Web ABM. Om du har köpt Web ABM efter september 2016 följer du stegen i [den här artikeln](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) i stället.

## Skapa en ny kontolista {#create-a-new-account-list-1}

1. Gå till **[!UICONTROL Account Lists]**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Välj **[!UICONTROL Create New]**.

   ![](assets/create-new-account-list-hand.jpg)

1. Välj **[!UICONTROL Browse]** och överför din CSV-fil (kontrollera att CSV-filen uppfyller villkoren). Lägg till en **[!UICONTROL List Name]** och **[!UICONTROL Description]**. Klicka på **[!UICONTROL Save]**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Vilket format har CSV-filen?**
   >
   >Kontrollera att CSV-filen för det namngivna kontot uppfyller följande krav:
   >
   >* Sparat som CSV-format
   >* överstiger inte 10 MB
   >* Endast fyra kolumner med rubriken Kolumn A: Namn, Kolumn B: Domän, Kolumn C: Land, Kolumn D: USA.
   >* Det kan ta upp till 2 arbetsdagar innan filen skickas för godkännande.
   >* Du får ett e-postmeddelande om godkännande eller en kontroll av filens status på sidan Namngivna konton.
   >* Det totala antalet poster/rader som ackumulerats för alla dina överförda listor börjar vid 10 000, med det största paketet på totalt 100 000.

   >[!NOTE]
   >
   >**Exempel på CSV-fil**
   >
   >* Rad 1 kolumn A värde = Organisation
   >* Rad 1 kolumn B värde = domän
   >* Rad 1 Kolumn C, värde = Land
   >* Rad 1 kolumn D värde = US State
   >* Ett av kolumnvärdena är obligatoriskt. Men om du anger både organisationsnamn och domännamn förbättras matchningsfrekvenserna i kontolistan.
   >* Land och stat är valfria värden.
   >
   >   * Använd det fullständiga landsnamnet eller förkortningskoden för landsnamnet. T.ex. USA.
   >   * För delstat i USA använder du förkortningskoden med två bokstäver, dvs. CA. Endast delstater i USA känns igen.
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Redigera en kontolista {#edit-an-account-list}

På sidan **Kontolistor** klickar du på ikonen **Redigera** i listan.

![](assets/create-new-account-list-edit.jpg)

Välj **[!UICONTROL Browse...]** och överför din nya CSV-fil. Den här filen ersätter originalfilen. Klicka på **[!UICONTROL Save]**. Den nya överförda filen kommer att vara i ett väntande läge tills den godkänts av Marketo Support, och när den är i ett väntande läge förblir den ursprungliga filen aktiv.

![](assets/set-account-list-edit-hands.jpg)

CSV-filen ersätter den befintliga filen. Den befintliga listan förblir aktiv tills bearbetningen av den nya filen är klar.

## Ta bort en namngiven kontolista {#delete-a-named-account-list}

1. På sidan **[!UICONTROL Account Lists]** klickar du på ikonen Ta bort för den lista du vill ta bort.

   ![](assets/create-new-account-list-delete.jpg)

1. Ett meddelande visas som bekräftar om du vill ta bort listan. Klicka på **[!UICONTROL OK]**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Skapa ett segment med en kontolista](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
