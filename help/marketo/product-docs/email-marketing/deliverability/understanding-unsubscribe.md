---
unique-page-id: 7514918
description: Så här säger du upp prenumerationen - Marketo Docs - produktdokumentation
title: Så här säger du upp prenumerationen
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Så här säger du upp prenumerationen {#understanding-unsubscribe}

Det finns faktiskt flera olika typer av inbyggda prenumerationer i Marketo. De representeras alla av fält på personobjektet, precis som förnamn.

Alla dessa fält är inbyggda i din Marketo-prenumeration. De är alla boolesk (kryssrutetyp). De kan användas i flödesstegen Forms eller [Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Avprenumererad {#unsubscribed}

Detta används på standardsidan för avanmälan. Om en person markerar den här rutan eller klickar på länken för att avbryta prenumerationen i ett e-postmeddelande får han/hon inte längre några marknadsföringsmeddelanden. De får dock [fungerande e-postmeddelanden](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marknadsföring har pausats {#marketing-suspended}

Det här fältet anges av användaren för att placera personer på en temporär avanmälan. Användarna kan bara uppnå den här statusen om de ändras manuellt eller om ett flödessteg för att ändra datavärdet används.

## E-post pausad {#email-suspended}

Den här statusen blockerar en person från att posta i 24 timmar efter att ett hårt studsfall har inträffat. Efter 24 timmar kommer personen att bli utskickbar igen.

>[!NOTE]
>
>Uppskjuten e-post kontrolleras även efter att 24-timmarsperioden är slut, så du kan hänvisa till personer som tidigare har markerats som sådana. För att se om personen kan mejlas behöver du bara beräkna 24 timmar efter det att du har stängt av e-postmeddelandet.

## Blocklist {#blocklisted}

[Använd detta för personer som konkurrenter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Alla som du vill ska få **no**-e-postmeddelanden - i drift, marknadsföring osv. De får ingenting!

![](assets/image2015-5-18-12-3a6-3a40.png)
