---
description: Loggning Sales Activity Attributes to Salesforce - Marketo Docs - Product Documentation
title: Loggar attribut för försäljningsaktivitet till Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 3%

---

# Loggar attribut för försäljningsaktivitet till [!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

Salesforce-administratör kan lägga till anpassade aktivitetsfält manuellt i [!DNL Salesforce].

1. Klicka på [!DNL Salesforce] i ditt **[!UICONTROL Setup]**-konto.

1. Sök efter&quot;Anpassade aktivitetsfält&quot; i snabbsökningsfältet och klicka på det.

1. Klicka på **[!UICONTROL New]**.

1. Välj datatyp som motsvarar fältet som du vill lägga till baserat på tabellen nedan och klicka på **[!UICONTROL Next]**.

1. Ange fältnamnet och etiketten för det fält som du vill lägga till.

Beskrivning av varje kolumn i tabellen nedan:

* **Fältetikett**: Fältnamn visas i användargränssnittet (det här namnet kan anpassas för att förbättra läsbarheten för ditt team)
* **Fältnamn**: Fältets tekniska namn (kontrollera att fältnamnet du anger matchar fältnamnet i tabellen nedan)
* **API-namn**: Det tekniska namnet på fältet för API (kontrollera att API-namnet du anger matchar API-namnet i tabellen nedan)
* **Datatyp**: Typ av fält
* **Storlek**: Textfältets storlek

<table>
 <tr>
  <th>Fältetikett</th>
  <th>Fältnamn</th>
  <th>API Name</th>
  <th>Datatyp</th>
  <th>Storlek</th>
 </tr>
  <tr>
  <td>[!UICONTROL Call Outcomes]</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result_c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Call Reasons]</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Text</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Local Presence ID]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Recording URL]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign Current Step]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign URL]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Attachment Viewed]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Clicked]</td>
  <td>MSE_Click</td>
  <td>MSE_Clicked_c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Replied]</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Status]</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Text</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Text</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template URL]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email URL]</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Viewed]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed_c</td>
  <td>Kryssruta</td>
  <td></td>
 </tr>
</table>
