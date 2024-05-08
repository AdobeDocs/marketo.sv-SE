---
unique-page-id: 10094576
description: Hållbart avbrutet abonnemang - Marketo Docs - produktdokumentation
title: Varaktigt avslut
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 35f5b33b01462b1cd00e29360daee465c7f18cf0
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Varaktigt avslut {#durable-unsubscribe}

Marketo har förbättrat beteendet för att avbryta prenumerationen så att den blir&quot;hållbar&quot;. Vi har lagt till en huvudstatus för e-post, som är skild från flaggan för att avbryta prenumerationen som visas på personinformationsposten.

Om flaggan för att avbryta prenumerationen är inställd på false uppdateras huvudens e-poststatus och ändringen sprids till andra personer med samma e-postadress. Om en person tas bort och återskapas, eller om en ny post skapas med samma e-postadress, kommer flaggan för att avbryta prenumerationen att **not** skrivas över.

>[!NOTE]
>
>Varaktigt Avbeställ fungerar för alla partitioner i hela Marketo-databasen.

## Uppdatera Unsubscribe Flag från True till False (t.ex. Resubscribe a Person) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Det finns flera sätt att återprenumerera på en person.

I Salesforce **clear** e-postavanmälningsfältet på lead/kontakts post. Detta synkroniseras med Marketo.

![](assets/one.png)

I MARKETO **clear** i rutan för att avbryta prenumerationen på fliken Info i personens post.

![](assets/two.png)

Kör en **Ändra datavärde** som visas nedan på en eller flera personer.

![](assets/three.png)

Uppdatera en befintlig person via SOAP API.

## Skapa en ny person {#creating-a-new-person}

När en ny person skapas kontrolleras den av Marketo mot huvudtabellen för e-poststatus. Om personen tidigare avbröt prenumerationen uppdaterar vi posten så att prenumerationen avbryts.

## Ändra en e-postadress {#changing-an-email-address}

Om du ändrar e-postadressen för en person till en e-postadress som du inte längre prenumererar på, kommer personen att avbeställa prenumerationen. Den här ändringen kan inträffa i antingen Marketo eller Salesforce.

Om du ändrar en e-postadress som du inte prenumererar på, kommer personen att prenumerera.

## Återprenumerera {#re-subscribing}

På samma sätt som ett avbrutet abonnemang skulle leda till att alla personer med samma e-postadress avbeställer prenumerationen skulle en återprenumeration faktiskt återbeställa alla personer med samma e-postadress.

>[!MORELIKETHIS]
>
>[Så här säger du upp prenumerationen](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
