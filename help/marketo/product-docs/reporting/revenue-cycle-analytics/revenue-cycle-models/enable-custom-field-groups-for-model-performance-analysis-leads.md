---
unique-page-id: 3571890
description: Aktivera anpassade fältgrupper för modellresultatanalys (leads) - Marketo Docs - produktdokumentation
title: Aktivera anpassade fältgrupper för modellresultatanalys (leads)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Aktivera anpassade fältgrupper för modellresultatanalys (leads) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Kategorisera standardfält eller anpassade fält i grupper för rapportering via Fältorganiseraren i Marketo. Mer information finns i [Skapa anpassade fältgrupper via fältorganiseraren](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

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
   <td colspan="1" rowspan="1"><p>Själva det anpassade fältet är aktiverat för rapportering i områdena Lead Analysis, Campaign Analysis och Opportunity Analysis.</p><p><strong>Obs! </strong> Anpassade fältgrupper stöds INTE i dessa analysområden, så gruppassociationerna visas inte i Inkomstcykelutforskaren, <em></em> bara i det anpassade fältet.</p></td> 
  </tr> 
 </tbody> 
</table>

Följ de här stegen för att aktivera en anpassad fältgrupp för rapportering i området för modellresultatanalys (Leads).

1. Klicka på **Admin**.

   ![](assets/one-1.png)

1. Klicka på **Intäktscykelanalys**.

   ![](assets/two-1.png)

1. Klicka på **Ingen** bredvid en tom fältgrupp. Om du redan har tre fältgrupper aktiverade och vill redigera, klickar du på namnet på fältgruppen som du vill ändra.

   ![](assets/three.png)

1. Klicka på listrutan **Fält** och välj det du vill använda.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >I det här exemplet aktiverades en anpassad fältgrupp för ett standardfält (tillstånd). Därför påverkades endast modellresultatanalysområdet (Leads). Om en anpassad fältgrupp för ett anpassat person- eller företagsfält hade aktiverats, skulle den aktiverade gruppen visas i avsnittet Modellresultatanalys (Leads) på fliken Synkroniseringssammanfattning och antalet anpassade fält för Lead-, Campaign- och Opportunity Analysis skulle öka med ett.

1. Klicka på **Spara**.

   ![](assets/five-1.png)
