---
unique-page-id: 7512979
description: Använda lead feed - Marketo Docs - produktdokumentation
title: Använda lead-feed
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# Använda lead-feed {#using-the-lead-feed}

Ledningsmataren är en uppdaterad lista över intressanta händelser som har utförts av dina leads. Du hittar den till höger när du klickar på fliken Marketo. Det är som en RSS- eller Twitter-feed - de senaste uppdateringarna finns högst upp i listan. Använd det här för att hoppa på leads medan du fortfarande är fräsch i deras sinnen.

>[!NOTE]
>
>Ledningsmatningen innehåller både de leads du äger och leads i din bevakningslista.

## Vad finns i huvudmatningen? {#whats-in-the-lead-feed}

![](assets/one.png)\
Varje objekt i lead-flödet är ett intressant ögonblick - en viktig aktivitet eller händelse i denna leads marknadsföringshistorik.

När du visar det i Salesforce har varje objekt:

![](assets/two.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><p>Objekt</p></td> 
   <td><p>Beskrivning</p></td> 
  </tr> 
  <tr> 
   <td><p>S. Lead/kontakt</p></td> 
   <td><p>Person som hade det här intressanta ögonblicket</p></td> 
  </tr> 
  <tr> 
   <td><p>B. Händelsetyp</p></td> 
   <td><p>Kategori för detta ögonblick - webb, e-post eller milstolpe</p></td> 
  </tr> 
  <tr> 
   <td><p>C. Kontonamn</p></td> 
   <td><p>Företag</p></td> 
  </tr> 
  <tr> 
   <td><p>D. Tid</p></td> 
   <td><p>När det här intressanta ögonblicket inträffade</p></td> 
  </tr> 
  <tr> 
   <td><p>E. Händelsebeskrivning</p></td> 
   <td><p>Orsak till detta intressanta ögonblick</p></td> 
  </tr> 
  <tr> 
   <td><p>F. Prenumerera</p></td> 
   <td><p>Få e-postmeddelanden för händelser som detta</p></td> 
  </tr> 
  <tr> 
   <td><p>G. Stjärna</p></td> 
   <td><p>Den här personen är ett Bästa val (hög prioritet)</p></td> 
  </tr> 
 </tbody> 
</table>

## Hämta RSS-uppdateringar {#getting-rss-updates}

Du kan också hämta uppdateringar för lead-feed via RSS-flöde.  Med en RSS-feed kan du få uppdateringar för dina leads även om du inte är ansluten till Salesforce. Flödet har samma information som lead-matningen i Salesforce samt följande (om den är tillgänglig):

* `email address`
* `phone number`
* `mobile number`
* `fax number`
* `company address`
* `company URL`

>[!NOTE]
>
>Företagets Marketo-administratör måste [aktivera RSS-flöden](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-configuration-tab/enable-rss-for-sales-insight.md) för att detta ska fungera.

För att få RSS-uppdateringar behöver du två saker: RSS-länken och en RSS-flödesläsare. Du kan få RSS-länken genom att klicka på RSS-ikonen i lead-flödet:   ![](assets/three.png)

RSS-flödet visas i ett nytt fönster. Du kan sedan kopiera URL:en för din RSS-feed och använda den i en RSS-läsare. De flesta webbläsare har en inbyggd RSS-läsare, eller så kan du använda en RSS-läsare som är specifik för din plattform.
