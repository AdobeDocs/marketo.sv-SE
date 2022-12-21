---
unique-page-id: 3571890
description: Aktivera anpassade fältgrupper för modellprestandaanalys (leads) - Marketo Docs - produktdokumentation
title: Aktivera anpassade fältgrupper för modellresultatanalys (leads)
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Aktivera anpassade fältgrupper för modellresultatanalys (leads) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Kategorisera standardfält eller anpassade fält i grupper för att rapportera via fältorganiseraren i Marketo. Mer information finns i [Skapa anpassade fältgrupper via fältorganiseraren](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>Hur påverkar aktivering av en anpassad fältgrupp flera analysområden i intäktscykelutforskaren?</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Vad händer när..?</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Hur det påverkar modellresultatanalysområdet (Leads)</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Hur det påverkar områdena Lead Analysis, Campaign Analysis och Opportunity Analysis</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Vad händer när du aktiverar en anpassad fältgrupp som är kopplad till ett standardlead- eller företagsfält?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Den anpassade fältgruppen är aktiverad för rapportering i modellresultatanalysområdet (Leads)</p></td> 
   <td colspan="1" rowspan="1"><p>Ingen effekt</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Vad händer när du aktiverar en anpassad fältgrupp som är kopplad till ett anpassat person- eller företagsfält?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Den anpassade fältgruppen är aktiverad för rapportering i modellresultatanalysområdet (Leads)</p></td> 
   <td colspan="1" rowspan="1"><p>Själva det anpassade fältet är aktiverat för rapportering i områdena Lead Analysis, Campaign Analysis och Opportunity Analysis.</p><p><strong>OBS!</strong> Anpassade fältgrupper stöds INTE i de här analysområdena, så gruppassociationerna visas inte i intäktscykelutforskaren—<em>endast</em> det anpassade fältet.</p></td> 
  </tr> 
 </tbody> 
</table>

Följ de här stegen för att aktivera en anpassad fältgrupp för rapportering i området för modellresultatanalys (Leads).

1. Klicka **Administratör**.

   ![](assets/one-1.png)

1. Klicka **Analys av intäktscykler**.

   ![](assets/two-1.png)

1. Klicka **Ingen** bredvid en tom fältgrupp. Om du redan har tre fältgrupper aktiverade och vill redigera, klickar du på namnet på fältgruppen som du vill ändra.

   ![](assets/three.png)

1. Klicka på **Fält** och välj den du vill använda.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >I det här exemplet aktiverades en anpassad fältgrupp för ett standardfält (tillstånd). Därför påverkades endast modellresultatanalysområdet (Leads). Om en anpassad fältgrupp för ett anpassat person- eller företagsfält hade aktiverats, skulle den aktiverade gruppen visas i avsnittet Modellresultatanalys (Leads) på fliken Synkroniseringssammanfattning och antalet anpassade fält för Lead-, Campaign- och Opportunity Analysis skulle öka med ett.

1. Klicka **Spara**.

   ![](assets/five-1.png)
