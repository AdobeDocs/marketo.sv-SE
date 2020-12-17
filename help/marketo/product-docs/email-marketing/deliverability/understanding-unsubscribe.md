---
unique-page-id: 7514918
description: Understanding Unsubscribe - Marketo Docs - produktdokumentation
title: Om att avbryta prenumerationen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Om att avbryta prenumeration {#understanding-unsubscribe}

Det finns faktiskt flera olika typer av inbyggda prenumerationer i Marketo. De representeras alla av fält på personobjektet, precis som förnamn.

>[!NOTE]
>
>Marketo håller på att ändra termer som Blacklist och Whitelist för att Blocklist och Tillåtslista i vår produkt. Under den här uppdateringen kan du se de gamla villkoren i våra användargränssnitt och skärmbilder för dokumentation samt de nya villkoren i vår dokumentationstext. Vi ber om ursäkt för all förvirring.

Alla dessa fält är inbyggda i er Marketo-prenumeration. De är alla boolesk (kryssrutetyp). De kan användas i flödesstegen Forms eller [Ändra datavärde](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Avbeställ {#unsubscribed}

Detta används på standardsidan för avanmälan. Om en person markerar den här rutan eller klickar på länken för att avbryta prenumerationen i ett e-postmeddelande får han/hon inte längre några marknadsföringsmeddelanden. De kommer dock att få [e-post om driften](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marknadsföring har pausats {#marketing-suspended}

Det här fältet anges av användaren för att placera personer på en temporär avanmälan. Användarna kan bara uppnå den här statusen om de ändras manuellt eller om ett flödessteg för att ändra datavärdet används.

## E-post pausad {#email-suspended}

Den här statusen blockerar en person från att posta i 24 timmar efter att ett hårt studsfall har inträffat. Efter 24 timmar kommer personen att bli utskickbar igen.

>[!NOTE]
>
>Uppskjuten e-post kontrolleras även efter att 24-timmarsperioden är slut, så du kan hänvisa till personer som tidigare har markerats som sådana. För att se om personen kan mejlas behöver du bara beräkna 24 timmar efter det att du har stängt av e-postmeddelandet.

## Blocklist {#blocklisted}

[Använd detta för personer som konkurrenter](http://docs.marketo.com/x/uwOQ). Alla du vill få **inga** e-postmeddelanden - i drift, marknadsföring osv. De får ingenting!

![](assets/image2015-5-18-12-3a6-3a40.png)

