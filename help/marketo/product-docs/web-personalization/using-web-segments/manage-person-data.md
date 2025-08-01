---
unique-page-id: 7504051
description: Hantera persondata - Marketo Docs - produktdokumentation
title: Hantera persondata
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 5%

---

# Hantera persondata {#manage-person-data}

Utnyttja persondata för [!DNL Web Personalization] genom att markera personfält som ska användas i din segmentering.

1. Gå till **[!UICONTROL Account Settings]**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. Gå till **[!UICONTROL Database]**.

   ![](assets/account-settings-dropdown-database.jpg)

## Lägga till ett fält för ny person {#adding-a-new-person-field}

1. Välj **Fält att lägga till** i listrutan för att lägga till ett persondatafält i listan.

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >Ett nytt fält läggs till i ett väntande läge och kan ta upp till 24 timmar att aktivera.

## Ta bort ett personfält {#deleting-a-person-field}

1. Klicka på borttagningsikonen ( ![—](assets/image2015-3-24-13-3a45-3a56.png)) för att ta bort ett fält från listan. Klicka på **[!UICONTROL Yes]** för att bekräfta att du vill ta bort fältet.

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**Hantera dina persondatafält**
   >
   >* Endast persondatafält kan inkluderas
   >* Du kan lägga till upp till 30 persondatafält
   >* Det kan ta upp till 24 timmar att aktivera nya fält
   >* Den maximala längden för strängtyper är 255 tecken
   >* Dolda fält tas bort automatiskt

<table>
 <tbody>
  <tr>
   <th><p>REST API-namn</p></th>
   <th><p>SOAP API-namn</p></th>
   <th><p>Eget namn</p></th>
  </tr>
  <tr>
   <td><p>avdelning</p></td>
   <td><p>Avdelning</p></td>
   <td><p>Avdelning</p></td>
  </tr>
  <tr>
   <td><p>title</p></td>
   <td><p>Titel</p></td>
   <td><p>Befattning</p></td>
  </tr>
  <tr>
   <td><p>värdering</p></td>
   <td><p>Klassificering</p></td>
   <td><p>Klassificering</p></td>
  </tr>
  <tr>
   <td><p>leadScore</p></td>
   <td><p>LeadScore</p></td>
   <td><p>Poäng</p></td>
  </tr>
  <tr>
   <td><p>leadStatus</p></td>
   <td><p>LeadStatus</p></td>
   <td><p>Status</p></td>
  </tr>
  <tr>
   <td><p>prioritet</p></td>
   <td><p>Prioritet</p></td>
   <td><p>Prioritet</p></td>
  </tr>
  <tr>
   <td><p>leadRole</p></td>
   <td><p>LeadRole</p></td>
   <td><p>Roll</p></td>
  </tr>
  <tr>
   <td><p>avbeställa</p></td>
   <td><p>Avprenumererad</p></td>
   <td><p>Avprenumererad</p></td>
  </tr>
 </tbody>
</table>

Följande lead-fält anges i rutan för nya [!DNL Web Personalization]-konton:

>[!MORELIKETHIS]
>
>[Skapa ett segment med kända persondata](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
