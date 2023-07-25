---
unique-page-id: 10094576
description: Hållbart avbrutet abonnemang - Marketo Docs - produktdokumentation
title: Varaktigt avslut
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Varaktigt avslut {#durable-unsubscribe}

Marketo har förbättrat beteendet för att avbryta prenumerationen så att den blir&quot;hållbar&quot;. Vi har lagt till en överordnad e-poststatus, som är skild från avregistreringsflaggan som visas på personinformationsposten.

Om flaggan för att avbryta prenumerationen är inställd på false uppdateras den överordnad e-poststatusen och ändringen sprids till andra personer med samma e-postadress. Om en person tas bort och återskapas, eller om en ny post skapas med samma e-postadress, kommer flaggan för att avbryta prenumerationen att **not** skrivas över.

>[!NOTE]
>
>Varaktigt Avbeställ fungerar för alla partitioner i hela Marketo-databasen.

## Uppdatera Unsubscribe Flag från True till False (t.ex. Resubscribe a Person) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Det finns flera sätt att återprenumerera på en person.

I Salesforce **clear** e-postavanmälningsfältet på lead/kontakts post. Detta synkroniseras med Marketo.

![](assets/one.png)

I Marketo **clear** i rutan för att avbryta prenumerationen på fliken Info i personens post.

![](assets/two.png)

Kör en **Ändra datavärde** som visas nedan på en eller flera personer.

![](assets/three.png)

Uppdatera en befintlig person via SOAP API.

## Skapa en ny person {#creating-a-new-person}

När en ny person skapas kontrollerar Marketo den mot den överordnad e-poststatustabellen. Om personen tidigare avbröt prenumerationen uppdaterar vi posten så att prenumerationen avbryts.

## Ändra en e-postadress {#changing-an-email-address}

Om du ändrar e-postadressen för en person till en e-postadress som du inte längre prenumererar på, kommer personen att avbeställa prenumerationen. Den här ändringen kan inträffa i antingen Marketo eller Salesforce.

Om du ändrar en e-postadress som du inte prenumererar på, kommer personen att prenumerera.

## Återprenumerera {#re-subscribing}

På samma sätt som ett avbrutet abonnemang skulle leda till att alla personer med samma e-postadress avbeställer prenumerationen skulle en återprenumeration faktiskt återbeställa alla personer med samma e-postadress.

## Aktivitetslogg {#activity-log}

Ändringsdefinitioner för datavärde för _updateLeadEmailStatus_ och _resetLeadEmailStatus_ finns i [den här communityartikeln](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Om att avbryta prenumerationen](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
