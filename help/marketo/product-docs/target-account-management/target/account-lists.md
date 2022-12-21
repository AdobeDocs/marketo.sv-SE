---
unique-page-id: 11378814
description: Kontolistor - Marketo Docs - produktdokumentation
title: Kontolistor
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Kontolistor {#account-lists}

En kontolista är en samling namngivna konton som kan användas tillsammans. Med kontolistor kan du rikta in namngivna konton efter bransch, plats eller storlek för företaget.

Förutom kontolistor kan du även skapa dynamiska kontolistor som genereras från offentliga CRM-kontovyer. En CRM-kontovy är en uppsättning regler som fungerar som ett filter när konton visas. Du kan till exempel använda den för att hitta konton där Branschen är hälsovård *och* Intäkterna är över 100 miljoner dollar.

![](assets/one.png)

>[!NOTE]
>
>Kontolistor som har skapats i Marketo Target Account Management är automatiskt tillgängliga när du skapar smarta listor och webbkampanjer i [Webbanpassning](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Skapa en ny kontolista {#create-a-new-account-list}

1. Klicka på **Nytt** nedrullningsbar meny och välj **Skapa ny kontolista**.

   ![](assets/1a.png)

1. Ge listan ett namn och klicka på **Skapa**.

   ![](assets/three-0.png)

1. När du har skapat din kontolista kan du börja på [lägga till namngivna konton](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo visar endast insikter för kontolistor med 2 000 eller färre namngivna konton.

## Skapa en ny dynamisk kontolista {#create-a-new-dynamic-account-list}

1. Klicka på **Nytt** nedrullningsbar meny och välj **Skapa ny dynamisk lista**.

   ![](assets/1.png)

1. I dialogrutan väljer du **CRM-kontovy** i listrutan eller skriv in namnet för att söka efter det.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicka **Skapa**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >I Salesforce måste du se till att du anger behörigheter för listvisningsobjekt till synkroniseringsanvändaren.

## Byta namn på en kontolista {#rename-an-account-list}

>[!NOTE]
>
>De här stegen gäller endast för kontolistor. _Dynamisk_ I kontolistor används namnet på deras associerade CRM-kontovyer.

1. Välj det konto du vill byta namn på och klicka på **Åtgärder för kontolista** nedrullningsbar meny och välj **Byt namn på kontolista**.

   ![](assets/three.png)

1. Ange det nya namnet och klicka på **Byt namn**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >CRM-kontovyn synkroniseras med den dynamiska kontolistan var 8:e timme. Om de inte har synkroniserats än synkroniseras de i Marketo under nästa cykel.

## Ta bort en kontolista {#delete-an-account-list}

>[!NOTE]
>
>De här stegen är desamma för både kontolistor och dynamiska kontolistor.

1. Markera kontot som du vill ta bort och klicka på **Åtgärder för kontolista** nedrullningsbar meny och välj **Ta bort kontolista**.

   ![](assets/five.png)

1. Klicka **Ta bort**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Lägg till ett befintligt namngivet konto i en kontolista](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Kontolisteinsikter](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)

