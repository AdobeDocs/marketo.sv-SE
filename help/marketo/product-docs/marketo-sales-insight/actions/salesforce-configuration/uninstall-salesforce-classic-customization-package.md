---
description: Avinstallera Salesforce Classic Customization Package - Marketo Docs - produktdokumentation
title: Avinstallera Salesforce Classic Customization Package
hide: true
hidefromtoc: true
exl-id: 17078054-a615-4f2f-bfde-f28fd3ff6f48
source-git-commit: 83556a56bddc1bdbeb5a5e93ec3a2c0d92aed831
workflow-type: tm+mt
source-wordcount: '1187'
ht-degree: 0%

---

# Avinstallera Salesforce Classic Customization Package {#uninstall-salesforce-classic-customization-package}

Avinstallera Marketo Sales Connect-paketet från ditt Salesforce-konto när du har börjat använda MSI-åtgärdspaketet.

## Ta bort Sales Connect-fält från sidlayout {#remove-sales-connect-fields-from-page-layout}

1. I Salesforce Classic klickar du på **Inställningar**.

   ![](assets/uninstall-salesforce-classic-customization-package-1.png)

1. Expandera (men klicka inte på) Anpassa under Skapa till vänster och sedan Leads. Välj sedan **Sidlayouter**.

   ![](assets/uninstall-salesforce-classic-customization-package-2.png)

1. Klicka **Redigera** bredvid Leadlayout.

   ![](assets/uninstall-salesforce-classic-customization-package-3.png)

1. I konsolen väljer du **Fält**. Sök efter MSC i Snabbsökning. Alla nedtonade fält har lagts till i sidlayouten. Du måste ta bort dem.

   ![](assets/uninstall-salesforce-classic-customization-package-4.png)

   >[!NOTE]
   >
   >Om inget av fälten är nedtonat betyder det att du inte har lagt till dem i sidlayouten. Du kan hoppa över det här avsnittet.

1. Bläddra till det avsnitt som innehåller anpassade fält för Sales Connect.

   ![](assets/uninstall-salesforce-classic-customization-package-5.png)

1. Det finns 10 typer av MSC-fält som kan läggas till i det här avsnittet. Ta bort alla fält som du har lagt till eller ta bort hela avsnittet.

1. Klicka **Snabbspara** när det är klart.

   ![](assets/uninstall-salesforce-classic-customization-package-6.png)

## Ta bort knappar för försäljningskontakt från sidlayouter {#remove-sales-connect-buttons-from-page-layouts}

1. I konsolen (steg 4 ovan) väljer du **Knappar**. Sök i MSC. Alla nedtonade knappar har lagts till i det anpassade knappavsnittet. Du måste ta bort dem.

   ![](assets/uninstall-salesforce-classic-customization-package-7.png)

   >[!NOTE]
   >
   >Om ingen av knapparna är nedtonad betyder det att du inte har lagt till dem. Du kan hoppa över det här avsnittet.

1. Dra och släpp MSC-knapparna från sektionen Anpassade knappar till konsolen.

   ![](assets/uninstall-salesforce-classic-customization-package-8.png)

1. Klicka **Snabbspara** när det är klart.

   ![](assets/uninstall-salesforce-classic-customization-package-9.png)

## Ta bort anslutningsfält för försäljning från avsnittet Aktivitetshistorik {#remove-sales-connect-fields-from-activity-history-section}

1. Bläddra längst ned på sidan till listavsnittet Aktivitetshistorik och klicka på ikonen för skiftnyckel.

   ![](assets/uninstall-salesforce-classic-customization-package-10.png)

1. Välj Koppla försäljning i området Markerade fält och klicka på pilen Ta bort. Klicka **OK** när det är klart.

   ![](assets/uninstall-salesforce-classic-customization-package-11.png)

   >[!NOTE]
   >
   >Förkortningen MSE _är_ Sales Connect. Det är bara det föregående namnet&quot;Marketo Sales Engage&quot;.

1. Klicka **Spara** när du är klar med sidan Leads.

## Ta bort åtgärdsknappar för Säljanslutning i grupp från leadlistevyn {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. Expandera (men klicka inte på) Anpassa under Skapa till vänster och sedan Leads. Välj sedan **Söklayouter**.

   ![](assets/uninstall-salesforce-classic-customization-package-12.png)

1. Klicka på bredvid listvyn Leads **Redigera**.

   ![](assets/uninstall-salesforce-classic-customization-package-13.png)

1. Välj **Lägg till i MSC Campaign (Classic)**, **E-post med MSC (Classic)** och **Skicka till MSC (klassisk)** och klicka på Ta bort-pilen. Klicka sedan på **Spara**.

   ![](assets/uninstall-salesforce-classic-customization-package-14.png)

Du bör inte längre se knapparna i leadlistevyn.

## Ta bort MSC-konfiguration för kontakter {#remove-msc-configuration-for-contacts}

1. I Salesforce klickar du på **Inställningar**.

1. Expandera (men klicka inte på) Anpassa under Build i den vänstra navigeringen och sedan Kontakter. Välj sedan **Sidlayouter**.

1. Klicka bredvid Kontaktlayout **Redigera**.

1. Upprepa steg från alla tre avsnitten.

## Ta bort MSC-konfiguration för affärsmöjlighet {#remove-msc-configuration-for-opportunity}

1. I Salesforce klickar du på **Inställningar**.

1. Utöka (men klicka inte på) Anpassa under Skapa i den vänstra navigeringsrutan, och sedan Affärsmöjligheter. Välj sedan **Sidlayouter**.

1. Klicka på bredvid säljprojektslayout **Redigera**.

1. Upprepa steg från alla tre avsnitten.

Affärsmöjlighetsvyn har bara en knapp -&quot;Skicka MSE-e-post&quot; och följande fält:

![](assets/uninstall-salesforce-classic-customization-package-15.png)

## Ta bort MSC-konfiguration för konto {#remove-msc-configuration-for-account}

1. I Salesforce klickar du på **Inställningar**.

1. Utöka (men klicka inte på) Anpassa under Build till vänster och sedan Konto. Välj sedan **Sidlayouter**.

1. Klicka på bredvid Kontolayout **Redigera**.

1. Upprepa steg från alla tre avsnitten.

Kontovyn har bara en knapp -&quot;Skicka MSE-e-post&quot; och följande fält:

![](assets/uninstall-salesforce-classic-customization-package-16.png)

## Ta bort Marketo Sales Outbox {#remove-marketo-sales-outbox}

1. I Salesforce klickar du på **+** överst på skärmen.

1. Klicka **Anpassa mina flikar**.

1. Välj alternativet Marketo Sales Outbox till höger. Klicka på borttagningspilen och sedan på **Spara**.

## Ta bort Sales Connect-paket {#delete-sales-connect-package}

När du har tagit bort alla objekt från ditt Salesforce-konto följer du stegen nedan.

1. I Salesforce klickar du på **Inställningar**.

1. Ange&quot;Apex Classes&quot; i rutan Snabbsökning.

1. Klicka **Ta bort** bredvid alla MarketoSalesConnectionCustomization- eller MarketoSalesEngageCustomization-poster i listan.

Allt är klart!

Här är en lista över alla objekt som behöver tas bort från Salesforce-instansen:

## Anpassningsinformation för Sales Connect {#sales-connect-customization-details}

<table>
 <tr>
  <th>Anpassade aktivitetsfält</th>
  <th>Beskrivning</th>
  <th>Typ</th>
  <th>Datatyp</th>
 </tr>
 <tr>
  <td>MSC-samtal Lokalt närvaro-ID</td>
  <td>Som användare kan jag välja Lokal närvaro som alternativ när jag ringer samtal från MSC Phone. Inkommande samtal visar ett lokalt nummer för mottagaren</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>URL för MSC-samtalsinspelning</td>
  <td>Samtal kan spelas in och en länk för inspelningen loggas här </td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC Campaign</td>
  <td>Loggnamn för MSC-kampanjen som kontakten/leadet är på</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>URL för MSC-kampanj</td>
  <td>Loggar URL till kampanjen som skapades i MSC. Om du klickar på detta öppnas kampanjen i MSC-webbappen</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>Aktuellt steg för MSC Campaign</td>
  <td>Om en kontakt/lead finns i en kampanj loggas namnet på steget som användaren är på</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
 <tr>
  <td>MSC-e-postbilaga visad</td>
  <td>Loggar data när ett e-postmeddelande skickas med en bifogad fil som visas av mottagaren</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
 <tr>
  <td>MSC-e-post klickad</td>
  <td>Loggar en bock när mottagaren klickar på en länk i e-postmeddelandet</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
 <tr>
  <td>MSC-e-postadress besvarad</td>
  <td>Loggar en bock när mottagaren svarar på e-postmeddelandet</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-e-poststatus</td>
  <td>Visar om ett e-postmeddelande skickas/håller på att skickas/studsas (spårning av studsade e-postmeddelanden beror på vilken leveranskanal som används)</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-e-postmall</td>
  <td>Loggnamn för MSC-mallen som användes i e-postmeddelandet som skickades till leadet/kontakten</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>URL för MSC-e-postmall</td>
  <td>Loggar URL till mallen som skapades i MSC. Om du klickar på det här öppnas mallen i MSC-webbprogrammet</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>URL för MSC-e-post</td>
  <td>Om du klickar på den här URL:en öppnas kommandocentralen i MSC och historikfliken med personinformationsvyn öppnas där användaren kan se det skickade e-postmeddelandet</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC-e-post visad</td>
  <td>Loggar en bockmarkering när mottagaren visar ett e-postmeddelande</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC-sammanslagningsloggningsfält</th>
  <th>Beskrivning</th>
  <th>Typ</th>
  <th>Datatyp</th>
 </tr>
 <tr>
  <td>MSC - senaste marknadsföringsåtagande</td>
  <td>Senaste inkommande engagemang från marknadsföring</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Data och tid</td>
 </tr>
 <tr>
  <td>MSC - datum för senaste marknadsföringsåtagande</td>
  <td>Tidstämpel för engagemang från marknadsföring</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Data och tid</td>
 </tr>
 <tr>
  <td>MSC - Senaste marknadsföringsbesök</td>
  <td>Beskrivning av engagemanget</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - källa för senaste marknadsföringsåtagande</td>
  <td>Källa för marknadsföringsengagemang</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - Typ av senaste marknadsföringsåtagande</td>
  <td>Typ av engagemang (t.ex.: Webbaktivitet)</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - senaste aktivitet per försäljning</td>
  <td>Senaste utgående aktivitet som utfördes av säljteamet</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Data och tid</td>
 </tr>
 <tr>
  <td>MSC - senaste svar</td>
  <td>Senaste e-postsvar till försäljning via e-post</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Data och tid</td>
 </tr>
 <tr>
  <td>MSC - aktuell försäljningskampanj</td>
  <td>Loggnamn för MSC-kampanjen som kontakten/leadet är på</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - senaste försäljningsåtagande</td>
  <td>Senaste inkommande ärende från försäljning</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Data och tid</td>
 </tr>
 <tr>
  <td>MSC - avanmäl dig</td>
  <td>Avanmäl dig från fält</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
  <td>Kryssruta</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC-knappar</th>
  <th>Beskrivning</th>
  <th>Typ</th>
 </tr>
 <tr>
  <td>Skicka MSC-e-post</td>
  <td>Skicka e-postmeddelanden från Salesforce</td>
  <td>
  <p>Konto 
  <p>Kontakt 
  <p>Lead 
  <p>Möjligheter</td>
 </tr>
 <tr>
  <td>Lägg till i MSC Campaign</td>
  <td>Lägg till i MSC-kampanjer från Salesforce</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>Skicka till MSC</td>
  <td>Skicka kontakt från Salesforce till MSC</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>Ring med MSC</td>
  <td>Ring säljsamtal från Salesforce</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
</table>

<table>
 <tr>
  <th>MSC-gruppåtgärdsknappar</th>
  <th>Beskrivning</th>
  <th>Typ</th>
 </tr>
 <tr>
  <td>Lägg till i MSC Campaign (Classic)</td>
  <td>Lägg till i MSC-kampanjer från Salesforce</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>Skicka till MSC (klassisk)</td>
  <td>Skicka kontakt från Salesforce till MSC</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>E-post med MSC (Classic)</td>
  <td>E-post med MSC från Salesforce</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
</table>
