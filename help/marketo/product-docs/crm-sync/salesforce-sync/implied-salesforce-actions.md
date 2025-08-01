---
unique-page-id: 4719304
description: Underförstådda Salesforce-åtgärder - Marketo Docs - produktdokumentation
title: Underförstådda Salesforce-åtgärder
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Underförstådda Salesforce-åtgärder {#implied-salesforce-actions}

När ett [!DNL Salesforce]-specifikt flödessteg körs, utförs ibland extra steg automatiskt. Här är reglerna, så du vet:

Dessa regler gäller när personen inte befinner sig i [Salesforce.com](https://Salesforce.com){target="_blank"} som kontakt eller lead.

<table>
 <thead>
  <tr>
   <th>Marketo Flow, steg</th>
   <th>Automatisk åtgärd</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Lägg till i SFDC Campaign</td>
   <td>Synkronisera person till SFDC</td>
  </tr>
  <tr>
   <td>Ändra status i SFDC Campaign</td>
   <td>Synkronisera person till SFDC<br>Lägg till i SFDC Campaign</td>
  </tr>
  <tr>
   <td>Ändra ägare</td>
   <td><p>Synkronisera person till SFDC</p></td>
  </tr>
  <tr>
   <td>Konvertera person</td>
   <td><p>Synkronisera person till SFDC</p></td>
  </tr>
  <tr>
   <td>Skapa uppgift</td>
   <td>Synkronisera person till SFDC</td>
  </tr>
 </tbody>
</table>

Du kan filtrera bort SFDC-poster i en smart lista med hjälp av filtret **[!UICONTROL SFDC Type]** med operatorn inställd på [!UICONTROL is not empty]. Alla SFDC-poster har ett värde i det här fältet.

Kom ihåg att dessa automatiska åtgärder bara utförs om leadet inte finns på [Salesforce.com](https://salesforce.com){target="_blank"}
