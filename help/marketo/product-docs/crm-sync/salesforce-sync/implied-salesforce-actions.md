---
unique-page-id: 4719304
description: Förstå vilka flödessteg i Salesforce som utlöser automatisk synkronisering av person till SFDC eller andra åtgärder. Lär dig reglerna för Lägg till i kampanj, Ändra ägare, Skapa aktivitet och Konvertera person.
title: Underförstådda Salesforce-åtgärder
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '157'
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
