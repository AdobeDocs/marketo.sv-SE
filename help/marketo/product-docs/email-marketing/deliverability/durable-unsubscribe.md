---
unique-page-id: 10094576
description: Hållbart avbrutet abonnemang - Marketo Docs - produktdokumentation
title: Varaktigt avslut
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Varaktigt avslut {#durable-unsubscribe}

Marketo har förbättrat beteendet för att avbryta prenumerationen så att den blir&quot;hållbar&quot;. Vi har lagt till en huvudstatus för e-post, som är skild från flaggan för att avbryta prenumerationen som visas på personinformationsposten.

Om flaggan för att avbryta prenumerationen är inställd på false uppdateras huvudens e-poststatus och ändringen sprids till andra personer med samma e-postadress. Om en person tas bort och återskapas, eller om en ny post skapas med samma e-postadress, skrivs flaggan för att avbryta prenumerationen **inte** över.

>[!NOTE]
>
>Varaktigt Avbeställ fungerar för alla partitioner i hela Marketo-databasen.

## Uppdatera Unsubscribe Flag från True till False (t.ex. Resubscribe a Person) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Det finns flera sätt att återprenumerera på en person.

I Salesforce rensar du fältet E-posta avanmälan på lead/kontakts post. Detta synkroniseras med Marketo.

![Salesforce-skärm](assets/durable-unsubscribe-1.png)

I Marketo avmarkerar du rutan för att avbryta prenumerationen på fliken Info i personposten.

![Rensar prenumerationsrutan i en personpost](assets/durable-unsubscribe-2.png)

Kör ett flödessteg för _Ändra datavärde_ så som visas nedan på en eller flera personer.

![Ändra flödessteg för datavärde](assets/durable-unsubscribe-3.png)

## Skapa en ny person {#creating-a-new-person}

När en ny person skapas kontrolleras den av Marketo mot huvudtabellen för e-poststatus. Om personen tidigare avbröt prenumerationen uppdaterar vi posten så att prenumerationen avbryts.

## Ändra en e-postadress {#changing-an-email-address}

Om du ändrar e-postadressen för en person till en e-postadress som du inte längre prenumererar på, kommer personen att avbeställa prenumerationen. Den här ändringen kan inträffa i antingen Marketo eller [!DNL Salesforce].

## Återprenumerera {#re-subscribing}

På samma sätt som ett avbrutet abonnemang skulle leda till att alla personer med samma e-postadress avbeställer prenumerationen skulle en återprenumeration faktiskt återbeställa alla personer med samma e-postadress.

>[!MORELIKETHIS]
>
>[Om att avbryta prenumerationen](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
