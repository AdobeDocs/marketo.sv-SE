---
unique-page-id: 14745793
description: Sales Connect-anpassningar för CRM - Marketo Docs - Produktdokumentation
title: Anpassningar av Sales Connect för CRM
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---


# Anpassningar av Sales Connect för CRM {#sales-connect-customizations-for-crm}

Fälten och knapparna nedan skapas av Metadata API i Salesforce CRM. När fälten har skapats måste administratörer konfigurera sidlayouterna i CRM så att de visas. Instruktioner finns [här](http://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Detta påverkar både ToutApp- och Sales Connect-kunder.

## Installera anpassningar i Salesforce {#how-to-install-customizations-in-salesforce}

1. Klicka på kugghjulsikonen i Sales Connect och välj **Inställningar**.

   ![](assets/one.png)

1. Välj **Salesforce** under Administratörsinställningar.

   ![](assets/two.png)

1. Klicka på **Marketo Sales Connect Customizations**.

   ![](assets/three.png)

1. Klicka på **Anslut till Salesforce**.

   ![](assets/four.png)

1. Logga in i Salesforce.

   ![](assets/five.png)

## Anpassade aktivitetsfält {#custom-activity-fields}

Marketo identifierar skapandet av de nya fälten och gör sedan en engångsefterfyllning av data, en ommappning och en pågående synkronisering av värden endast i de **nya** fälten. Gamla fält uppdateras inte.

| **Fältnamn** | **Beskrivning** |
|---|---|
| MSE-anrop av lokalt närvaro-ID | Som användare kan du välja Lokal närvaro som alternativ när du ringer från MSE-telefonen. Inkommande samtal visar ett lokalt nummer för mottagaren. |
| URL för MSE-samtalsinspelning | Samtal kan spelas in och en länk för inspelningen loggas här. |
| MSE Campaign | Loggnamn för den MSE-kampanj som kontakten/ledningen är medlem i. |
| MSE Campaign URL | Loggar URL till kampanjen som skapades i MSE. Om du klickar på detta öppnas kampanjen i MSE-webbappen. |
| Aktuellt steg för MSE-kampanj | Om en kontakt/lead är en del av en kampanj loggas namnet på det steg som leadet/kontakten är aktiverad för. |
| MSE E-postbilaga visad | Loggar data när ett e-postmeddelande skickas med en bifogad fil och den bifogade filen visas av mottagaren. |
| MSE-e-post klickad | Loggar en bock när mottagaren klickar på en länk i ett e-postmeddelande. |
| MSE-e-postadress besvarad | Loggar en bock när mottagaren svarar på ett e-postmeddelande. |
| MSE-e-poststatus | Visar om ett e-postmeddelande skickas/håller på att skickas/studsas (spårning av studsade e-postmeddelanden beror på vilken leveranskanal som används). |
| MSE-e-postmall | Loggar namnet på MSE-mallen som användes i e-postmeddelandet som skickades till leadet/kontakten. |
| URL för MSE-e-postmall | Loggar URL till mallen som skapades i MSE. Om du klickar på den öppnas mallen i MSE-webbprogrammet. |
| MSE-e-post-URL | Om du klickar på den här URL:en öppnas Kommando Center i MSE och fliken Historik för personinformationsvyn öppnas där du kan se det skickade e-postmeddelandet. |
| MSE-e-post visad | Loggar en bock när mottagaren visar ett e-postmeddelande. |

## Sammanslagning av loggningsfält {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Fältnamn</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>MSE - Senaste marknadsföringsåtagande</td> 
   <td>Senaste inkommande engagemang från marknadsföring. </td> 
  </tr> 
  <tr> 
   <td>MSE - Senaste marknadsföringsdatum</td> 
   <td>Tidstämpel för engagemang från marknadsföring.</td> 
  </tr> 
  <tr> 
   <td>MSE - Senaste marknadsföringsbesök</td> 
   <td>Beskrivning av engagemanget.</td> 
  </tr> 
  <tr> 
   <td>MSE - Senaste marknadsföringsaktivitetskälla</td> 
   <td>Källa för marknadsföringsengagemang.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Typ av senaste marknadsföringsåtagande</td> 
   <td colspan="1">Typ av engagemang.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Senaste aktivitet per försäljning<br></td> 
   <td colspan="1">Senaste utgående aktivitet som utfördes av säljteamet.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Senaste svar</td> 
   <td colspan="1">Senaste e-postsvar till e-postmeddelandet.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Aktuell försäljningskampanj</td> 
   <td colspan="1">Loggnamn för MSE-kampanjen som leadet/kontakten är medlem i.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Senaste försäljningsåtagande</td> 
   <td colspan="1">Senaste inkommande ärende från försäljning. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Avanmäl dig</td> 
   <td colspan="1">Avanvisningsfält.</td> 
  </tr> 
 </tbody> 
</table>

## Knappar {#buttons}

| **Knappnamn** | **Beskrivning** |
|---|---|
| Skicka MSE-e-post | Skicka e-postmeddelanden från Salesforce. |
| Lägg till i MSE-kampanj | Lägg till MSE-kampanjer från Salesforce. |
| Skjut till MSE | Skicka kontakt från Salesforce till MSE. |
| Samtal med MSE | Ring säljsamtal från Salesforce. |

## Knappar för gruppåtgärd {#bulk-action-buttons}

| **Knappnamn** | **Beskrivning** |
|---|---|
| Lägg till i MSE-kampanj | Lägg till MSE-kampanjer från Salesforce. |
| Skjut till MSE | Skicka kontakt från Salesforce till MSE. |

## Användarhandböcker {#user-guides}

[Anpassade MSE-rapporter i Salesforce](http://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE för Salesforce](http://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE för Salesforce Lightning](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)

## Relaterade videoklipp {#related-videos}

**Installera anpassningar i Salesforce**
`<iframe width="630" height="470" src="//play.vidyard.com/YEPWYBfFEa4nKCo2F6bKKc.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>` ** Fördelen med att använda anpassningar i Salesforce** 
`<iframe width="630" height="470" src="//play.vidyard.com/4PzSDb6o8Qg8WbvBsq8wJD.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`