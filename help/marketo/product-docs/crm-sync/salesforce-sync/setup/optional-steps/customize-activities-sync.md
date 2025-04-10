---
unique-page-id: 4719294
description: Synkronisera anpassade aktiviteter - Marketo Docs - Produktdokumentation
title: Synkronisera anpassade aktiviteter
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Synkronisera anpassade aktiviteter {#customize-activities-sync}

Om du inte använder Marketo Sales Insight kan Marketo Engage skapa Salesforce Activity History Records för vissa händelser. Så här aktiverar du dem.

>[!NOTE]
>
>Salesforce/Marketo Engage-synkroniseringen kommer inte att skicka några aktiviteter till Salesforce som inträffade innan personen överfördes till Salesforce.

1. Gå till **[!UICONTROL Admin]**.

   ![](assets/customize-activities-sync-1.png)

1. Klicka på **[!DNL Salesforce]** och sedan på **[!UICONTROL Edit Sync Options]**.

   ![](assets/two-1.png)

1. Markera rutorna intill aktiviteter som du vill att Marketo ska skicka till Salesforce och klicka på **[!UICONTROL Save]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >När Marketo väl har aktiverats kommer det att gå tre månader framåt i aktivitetshistoriken. Beroende på mängden data kan _det här ta flera dagar att slutföra_. Uppdateringar som inträffar under den initiala aktivitetspush-åtgärden kan fördröjas tills den initiala aktivitetssynkroniseringen har slutförts.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Typ av aktivitet</th> 
   <th>Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ifyllt formulär</td> 
   <td>Fyll i alla Marketo-formulär</td> 
  </tr> 
  <tr> 
   <td>Tillagd i listan</td> 
   <td><p>Flödessteg: lades till i en statisk lista</p></td> 
  </tr> 
  <tr> 
   <td>E-post skickad</td> 
   <td>Flödessteg: Skickades ett e-postmeddelande</td> 
  </tr> 
  <tr> 
   <td>E-post levererad</td> 
   <td>Har tagit emot ett e-postmeddelande (inte studsat)</td> 
  </tr> 
  <tr> 
   <td>E-post öppnad</td> 
   <td>Öppnade ett e-postmeddelande (utan blockerade bilder)</td> 
  </tr> 
  <tr> 
   <td>Klicka på länken i e-postmeddelandet</td> 
   <td>Klicka på en länk i ett e-postmeddelande som skickats av Marketo</td> 
  </tr> 
  <tr> 
   <td>Borttagen från listan</td> 
   <td>Flödessteg: togs bort från en statisk lista</td> 
  </tr> 
  <tr> 
   <td>Ta bort från flöde</td> 
   <td>Flödessteg: Ta bort från flöde</td> 
  </tr> 
  <tr> 
   <td>E-postmeddelande har skickats</td> 
   <td>Skickades via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-postadress öppnad</td> 
   <td>Öppnade ett e-postmeddelande som skickats via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Klicka på länken i försäljningsmejl</td> 
   <td>Klicka på en länk i ett e-postmeddelande som skickats via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-postmeddelande har tagits emot</td> 
   <td>Ett e-postmeddelande togs emot och loggades av säljaren i MSI Outlook-plugin-programmet</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;E-postförsäljning mottagen&quot; innebär _inte_ levererad. Leveransstatus hämtas inte för e-postmeddelanden som skickas via Sales Insight.

>[!TIP]
>
>Om du är intresserad av att få in mer information om Marketo i Salesforce kan du ta en titt på vår [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} -produkt.
