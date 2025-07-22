---
unique-page-id: 14745793
description: '[!DNL Sales Connect] anpassningar för CRM - Marketo Docs - produktdokumentation'
title: '[!DNL Sales Connect] anpassningar för CRM'
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 1%

---

# [!DNL Sales Connect] anpassningar för CRM {#sales-connect-customizations-for-crm}

Fälten och knapparna nedan skapas av Metadata API i Salesforce CRM. När fälten har skapats måste administratörer konfigurera sidlayouterna i CRM så att de visas. Instruktionerna [finns här](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Installera anpassningar i [!DNL Salesforce] {#how-to-install-customizations-in-salesforce}

1. Klicka på kugghjulsikonen i [!DNL Sales Connect] och välj **[!UICONTROL Settings]**.

   ![](assets/one.png)

1. Välj [!UICONTROL Admin Settings] under **[!UICONTROL Salesforce]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Marketo Sales Engage Customizations]**.

   ![](assets/three.png)

1. Klicka på **[!UICONTROL Connect to Salesforce]**.

   ![](assets/four.png)

1. Logga in på [!DNL Salesforce].

   ![](assets/five.png)

## Uppdatera anpassning av [!DNL Salesforce] {#update-salesforce-customization}

Uppdateringar av anpassningspaketet [!DNL Salesforce] innehåller förbättringar och felkorrigeringar. Följ stegen nedan för att kontrollera om det finns uppdateringar eller för att utföra en uppdatering.

>[!NOTE]
>
>**Administratörsbehörighet krävs.**

1. Klicka på kugghjulsikonen i [webbprogrammet](https://www.toutapp.com) och välj **[!UICONTROL Settings]**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL Salesforce]**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Anpassningskortet [!DNL Sales Connect] visas om det finns tillgängliga uppdateringar. Klicka på **[!UICONTROL Update Customizations]**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Klicka på **[!UICONTROL Upgrade]**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Vänta tills uppdateringarna har installerats. Installationstiden varierar beroende på hur många versionsnummer du behöver.

   ![](assets/sales-connect-customizations-for-crm-10.png)

När kortet är klart visas&quot;Säljarens anpassningar av Connect är uppdaterade.&quot;

![](assets/sales-connect-customizations-for-crm-11.png)

## Anpassade aktivitetsfält {#custom-activity-fields}

Marketo upptäcker att de nya fälten har skapats och gör sedan en engångsefterfyllning av data, en ommappning och en pågående synkronisering av värden endast i fälten **new**. Gamla fält uppdateras inte.

<table><thead>
  <tr>
    <th>Fältnamn</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE-anrop av lokalt närvaro-ID</td>
    <td>Som användare kan du välja Lokal närvaro som alternativ när du ringer från MSE-telefonen. Inkommande samtal visar ett lokalt nummer för mottagaren.</td>
  </tr>
  <tr>
    <td>URL för MSE-samtalsinspelning</td>
    <td>Samtal kan spelas in och en länk för inspelningen loggas här.</td>
  </tr>
  <tr>
    <td>MSE Campaign</td>
    <td>Loggnamn för den MSE-kampanj som kontakten/ledningen är medlem i.</td>
  </tr>
  <tr>
    <td>MSE Campaign URL</td>
    <td>Loggar URL till kampanjen som skapades i MSE. Om du klickar på detta öppnas kampanjen i MSE-webbappen.</td>
  </tr>
  <tr>
    <td>Aktuellt steg för MSE-kampanj</td>
    <td>Om en kontakt/lead är en del av en kampanj loggas namnet på det steg som leadet/kontakten är aktiverad för.</td>
  </tr>
  <tr>
    <td>MSE E-postbilaga visad</td>
    <td>Loggar data när ett e-postmeddelande skickas med en bifogad fil och den bifogade filen visas av mottagaren.</td>
  </tr>
  <tr>
    <td>MSE-e-post klickad</td>
    <td>Loggar en bock när mottagaren klickar på en länk i ett e-postmeddelande.</td>
  </tr>
  <tr>
    <td>MSE-e-postadress besvarad</td>
    <td>Loggar en bock när mottagaren svarar på ett e-postmeddelande.</td>
  </tr>
  <tr>
    <td>MSE-e-poststatus</td>
    <td>Visar om ett e-postmeddelande skickas/håller på att skickas/studsas (spårning av studsade e-postmeddelanden beror på vilken leveranskanal som används).</td>
  </tr>
  <tr>
    <td>MSE-e-postmall</td>
    <td>Loggar namnet på MSE-mallen som användes i e-postmeddelandet som skickades till leadet/kontakten.</td>
  </tr>
  <tr>
    <td>URL för MSE-e-postmall</td>
    <td>Loggar URL till mallen som skapades i MSE. Om du klickar på den öppnas mallen i MSE-webbprogrammet.</td>
  </tr>
  <tr>
    <td>MSE-e-post-URL</td>
    <td>Om du klickar på den här URL:en öppnas Kommando Center i MSE och fliken Historik för personinformationsvyn öppnas där du kan se det skickade e-postmeddelandet.</td>
  </tr>
  <tr>
    <td>MSE-e-post visad</td>
    <td>Loggar en bock när mottagaren visar ett e-postmeddelande.</td>
  </tr>
</tbody></table>

## Samla in loggningsfält {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Fältnamn</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - Senaste marknadsföringsåtagande</td>
    <td>Senaste inkommande engagemang från marknadsföring.</td>
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
    <td>MSE - Last Marketing Engagement Source</td>
    <td>Source om marknadsföringsengagemang.</td>
  </tr>
  <tr>
    <td>MSE - Typ av senaste marknadsföringsåtagande</td>
    <td>Typ av engagemang.</td>
  </tr>
  <tr>
    <td>MSE - Senaste aktivitet per försäljning</td>
    <td>Senaste utgående aktivitet som utfördes av säljteamet.</td>
  </tr>
  <tr>
    <td>MSE - Senaste svar</td>
    <td>Senaste e-postsvar till e-postmeddelandet.</td>
  </tr>
  <tr>
    <td>MSE - Aktuell försäljningskampanj</td>
    <td>Loggnamn för MSE-kampanjen som leadet/kontakten är medlem i.</td>
  </tr>
  <tr>
    <td>MSE - Senaste försäljningsåtagande</td>
    <td>Senaste inkommande ärende från försäljning.</td>
  </tr>
  <tr>
    <td>MSE - Avanmäl dig</td>
    <td>Avanvisningsfält.</td>
  </tr>
</tbody></table>

## Knappar {#buttons}

<table><thead>
  <tr>
    <th>Knappnamn</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Skicka MSE-e-post</td>
    <td>Skicka e-postmeddelanden från Salesforce.</td>
  </tr>
  <tr>
    <td>Lägg till i MSE-kampanj</td>
    <td>Lägg till MSE-kampanjer från Salesforce.</td>
  </tr>
  <tr>
    <td>Skjut till MSE</td>
    <td>Skicka kontakt från Salesforce till MSE.</td>
  </tr>
  <tr>
    <td>Samtal med MSE</td>
    <td>Ring Salesforce.</td>
  </tr>
</tbody>
</table>

## Knappar för gruppåtgärd {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Knappnamn</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Lägg till i MSE-kampanj</td>
    <td>Lägg till MSE-kampanjer från Salesforce.</td>
  </tr>
  <tr>
    <td>Skjut till MSE</td>
    <td>Skicka kontakt från Salesforce till MSE.</td>
  </tr>
</tbody>
</table>

## Användarhandböcker {#user-guides}

[Anpassade MSE-rapporter i Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE för Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE för Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
