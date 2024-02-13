---
unique-page-id: 3571844
description: Microsoft Dynamics Sync -Opportunity Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - säljprojektssynkronisering
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Affärsmöjlighet synkroniserad {#microsoft-dynamics-sync-opportunity-sync}

Synkroniseringen mellan Marketo Engage och Dynamics är superkraftfull. Här är all information för affärsmöjlighetssynkronisering.

## Hur synkroniseras informationen om affärsmöjligheterna mellan de två systemen? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Affärsmöjligheterna synkroniseras på ett sätt - Dynamics till Marketo. Om du ändrar en affärsmöjlighet i Dynamics återspeglas uppdateringen i Marketo.

## Kan jag skapa en affärsmöjlighet i Dynamics med Marketo? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Nej, du måste skapa affärsmöjligheten i Dynamics och den synkroniseras automatiskt till Marketo.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [markera fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} under installationen.

## Hur är ett konto/en kontakt associerad med ett säljprojekt? {#how-is-an-account-contact-associated-with-an-opportunity}

Kontakten/kontot kan kopplas till säljprojekt på två sätt:

* När du skapar en affärsmöjlighet kan du ange kontaktfält (sökfält i formuläret som ska kontaktas) och/eller konto (sökfält i formuläret till konto). I båda fallen lagras dessa värden i fältet Potential Customer (customerid) i Dynamics. Det här fältet visas inte i formuläret för affärsmöjlighet, men kan läggas till från inställningarna. Det här fältet kan bara innehålla 1 värde, antingen kontakt eller konto. Marketo gör följande:

   * Om kontaktvärdet anges och kontot lämnas tomt skapar Marketo en `opportunitycontactrole` och anger kontot för affärsmöjligheten till kontaktens konto. Om kontakten inte har något konto lämnas fältet tomt.
   * Om kontovärdet anges och kontakten lämnas tom, kommer Marketo endast att ställa in kontot för affärsmöjligheten på det här kontot.
   * Om båda värdena anges väljs kontot som värde för kundens ID, vilket innebär att beteendet är detsamma som ovan.


* Via intressenter: Dynamics använder anslutningar för att koppla samman möjligheter till kontakt via intressenter från skapandesidan för affärsmöjligheter. För detta kommer vi att skapa en `opportunitycontactrole` för varje ny berörd part.
