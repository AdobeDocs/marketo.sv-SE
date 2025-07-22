---
unique-page-id: 11378814
description: '[!UICONTROL Account Lists] - Marketo Docs - produktdokumentation'
title: '[!UICONTROL Account Lists]'
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# [!UICONTROL Account Lists] {#account-lists}

En kontolista är en samling namngivna konton som kan användas tillsammans. Med kontolistor kan du rikta in namngivna konton efter bransch, plats eller storlek för företaget.

Förutom kontolistor kan du även skapa dynamiska kontolistor som genereras från offentliga CRM-kontovyer. En CRM-kontovy är en uppsättning regler som fungerar som ett filter när konton visas. Du kan till exempel använda den för att hitta konton där Bransch är hälsovård *och* intäkter är över 100 miljoner USD.

![](assets/one.png)

>[!NOTE]
>
>Kontolistor som har skapats i Marketo [!UICONTROL Target Account Management] är automatiskt tillgängliga när du skapar smarta listor och webbkampanjer i [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Skapa en ny kontolista {#create-a-new-account-list}

1. Klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL Create New Account List]**.

   ![](assets/1a.png)

1. Ge listan ett namn och klicka på **[!UICONTROL Create]**.

   ![](assets/three-0.png)

1. När du har skapat din kontolista börjar du [lägga till namngivna konton i den](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo visar endast insikter för kontolistor med 2 000 eller färre namngivna konton.

## Skapa en ny dynamisk kontolista {#create-a-new-dynamic-account-list}

1. Klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL Create New Dynamic List]**.

   ![](assets/1.png)

1. I dialogrutan väljer du en **CRM-kontovy** i listrutan eller skriver namnet som du vill söka efter.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >I Salesforce måste du ange behörigheter för listvisningsobjekt till synkroniseringsanvändaren.

## Byta namn på en kontolista {#rename-an-account-list}

>[!NOTE]
>
>De här stegen gäller endast för kontolistor. _Dynamiska_-kontolistor använder namnet på deras associerade CRM-kontovyer.

1. Välj det konto du vill byta namn på, klicka på listrutan **[!UICONTROL Account List Actions]** och välj **[!UICONTROL Rename Account List]**.

   ![](assets/three.png)

1. Ange det nya namnet och klicka på **[!UICONTROL Rename]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >CRM-kontovyn synkroniseras med den dynamiska kontolistan var 8:e timme. Om de inte har synkroniserats än synkroniseras de i Marketo under nästa cykel.

## Ta bort en kontolista {#delete-an-account-list}

>[!NOTE]
>
>De här stegen är desamma för både kontolistor och dynamiska kontolistor.

1. Markera det konto som du vill ta bort, klicka på listrutan **[!UICONTROL Account List Actions]** och välj **[!UICONTROL Delete Account List]**.

   ![](assets/five.png)

1. Klicka på **[!UICONTROL Delete]**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Lägg till en befintlig [!UICONTROL Named Account] i en kontolista](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Kontolisteinsikter](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
