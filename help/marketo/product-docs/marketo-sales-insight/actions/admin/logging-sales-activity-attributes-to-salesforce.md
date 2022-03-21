---
description: Loggning Sales Activity Attributes to Salesforce - Marketo Docs - Product Documentation
title: Loggningsattribut för försäljningsaktivitet till Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Loggningsattribut för försäljningsaktivitet till Salesforce {#logging-sales-activity-attributes-to-salesforce}

Salesforce-administratör kan lägga till anpassade aktivitetsfält manuellt i Salesforce.

1. Klicka på i Salesforce-kontot **Inställningar**.

1. Sök efter&quot;Anpassade aktivitetsfält&quot; i snabbsökningsfältet och klicka på det.

1. Klicka **Nytt**.

1. Välj den datatyp som motsvarar fältet som du vill lägga till baserat på tabellen nedan och klicka på **Nästa**.

1. Ange fältnamnet och etiketten för det fält som du vill lägga till.

Beskrivning av varje kolumn i tabellen nedan:

* **Fältetikett**: Fältnamn som visas i användargränssnittet (det här namnet kan anpassas för att förbättra läsbarheten för ditt team)
* **Fältnamn**: Fältets tekniska namn (kontrollera att fältnamnet du anger matchar fältnamnet i tabellen nedan)
* **API-namn**: Tekniskt namn på fältet för API (se till att API-namnet som du anger matchar API-namnet i tabellen nedan)
* **Datatyp**: Typ av fält
* **Storlek**: Textfältets storlek

<table>
 <tr>
  <th>Fältetikett</th>
  <th>Fältnamn</th>
  <th>API-namn</th>
  <th>Datatyp</th>
  <th>Storlek</th>
 </tr>
 <tr>
  <td>Marketo-samtal Lokalt närvaro-ID</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo URL för samtalsinspelning</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo Sales Campaign</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo Sales Campaign - aktuellt steg</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo Sales Campaign URL</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>E-postbilaga för Marketo försäljning visad</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo Sales Email Click</td>
  <td>MSE_Click</td>
  <td>MSE_Clicked_c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo-e-postadress - svar</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
 <tr>
  <td>E-poststatus för Marketo</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Text</td>
  <td></td>
 </tr>
 <tr>
  <td>E-postmall för Marketo</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL för Marketo E-postmall</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo Sales Email URL</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>E-post från Marketo visad</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed_c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
</table>
