---
unique-page-id: 3571890
description: Aktivera anpassade fältgrupper för modellprestandaanalys (leads) - Marketo Docs - produktdokumentation
title: Aktivera anpassade fältgrupper för modellresultatanalys (leads)
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '325'
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
   <td colspan="1" rowspan="1"><p><strong>Så här påverkar det <span class="uicontrol">modellprestandaanalysområdet (Leads)</span></strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>Hur det påverkar områdena Lead Analysis, Campaign Analysis och Opportunity Analysis</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Vad händer när du aktiverar en anpassad fältgrupp som är kopplad till ett standardlead- eller företagsfält?</strong></p></td>
   <td colspan="1" rowspan="1"><p>Den anpassade fältgruppen är aktiverad för rapportering i området <span class="uicontrol">Modellresultatanalys (Leads)</span></p></td>
   <td colspan="1" rowspan="1"><p>Ingen effekt</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Vad händer när du aktiverar en anpassad fältgrupp som är kopplad till ett anpassat person- eller företagsfält?</strong></p></td>
   <td colspan="1" rowspan="1"><p>Den anpassade fältgruppen är aktiverad för rapportering i området <span class="uicontrol">Modellresultatanalys (Leads)</span></p></td>
   <td colspan="1" rowspan="1"><p>Själva det anpassade fältet är aktiverat för rapportering i områdena Lead Analysis, Campaign Analysis och Opportunity Analysis.</p><p><strong>OBS!</strong> Anpassade fältgrupper stöds INTE i de här analysområdena, så gruppassociationerna visas inte i Inkomstcykelutforskaren -<em>endast</em> det anpassade fältet.</p></td>
  </tr>
 </tbody>
</table>

Följ de här stegen för att aktivera en anpassad fältgrupp för rapportering i området [!UICONTROL Model Performance Analysis (Leads)].

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/one-1.png)

1. Klicka på **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/two-1.png)

1. Klicka på **[!UICONTROL None]** bredvid en tom fältgrupp. Om du redan har tre fältgrupper aktiverade och vill redigera, klickar du på namnet på fältgruppen som du vill ändra.

   ![](assets/three.png)

1. Klicka på listrutan **[!UICONTROL Field]** och välj den du vill använda.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >I det här exemplet aktiverades en anpassad fältgrupp för ett standardfält (tillstånd). Därför påverkades bara området [!UICONTROL Model Performance Analysis (Leads)]. Om en anpassad fältgrupp för ett anpassat person- eller företagsfält hade aktiverats, skulle den aktiverade gruppen visas i avsnittet [!UICONTROL Model Performance Analysis (Leads)] på fliken Synkroniseringssammanfattning och antalet anpassade fält för Lead-, Campaign- och Opportunity Analysis skulle öka med ett.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/five-1.png)
