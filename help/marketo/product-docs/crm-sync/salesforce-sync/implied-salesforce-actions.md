---
unique-page-id: 4719304
description: Underförstådda Salesforce-åtgärder - Marketo Docs - produktdokumentation
title: Underförstådda Salesforce-åtgärder
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Underförstådda Salesforce-åtgärder {#implied-salesforce-actions}

När ett Salesforce-specifikt flödessteg körs, utförs ibland extra steg automatiskt. Här är reglerna, så du vet:

Dessa regler gäller _när personen inte är närvarande [Salesforce.com](https://Salesforce.com)_ som kontakt eller lead.

<table> 
 <thead> 
  <tr> 
   <th>Marketo Flow</th> 
   <th>Automatisk åtgärd</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Lägg till i SFDC-kampanj</td> 
   <td>Synkronisera person till SFDC</td> 
  </tr> 
  <tr> 
   <td>Ändra status i SFDC-kampanj</td> 
   <td>Synkronisera person till SFDC<br>Lägg till i SFDC-kampanj</td> 
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

Du kan filtrera bort SFDC-poster i en smart lista med hjälp av **SFDC-typ** Filtrera med operatorn inställd på &quot;är inte tom&quot;. Alla SFDC-poster har ett värde i det här fältet.

Kom ihåg att dessa automatiska åtgärder bara utförs om leadet inte finns i [Salesforce.com](https://salesforce.com)
