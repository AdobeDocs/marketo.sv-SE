---
description: Avinstallera Salesforce Lightning Customization Package - Marketo Docs - produktdokumentation
title: Avinstallera Salesforce Lightning Customization Package
exl-id: 4af89222-22b1-4c08-8081-3dab89d1985b
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 5%

---

# Avinstallera anpassningspaketet för [!DNL Salesforce Lightning] {#uninstall-salesforce-lightning-customization-package}

Avinstallera Marketo [!DNL Sales Connect]-paketet från ditt [!DNL Salesforce]-konto när du har börjat använda MSI-åtgärdspaketet.

## Ta bort [!DNL Sales Connect] fält från sidlayout {#remove-sales-connect-fields-from-page-layout}

1. Klicka på kugghjulsikonen i [!DNL Salesforce Lightning] och välj **[!UICONTROL Setup]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-1.png)

1. Klicka på **[!UICONTROL Object Manager]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-2.png)

1. Rulla ned till och välj **[!UICONTROL Lead]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-3.png)

1. Klicka på **[!UICONTROL Page Layouts]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-4.png)

1. Klicka på **[!UICONTROL Lead Layout]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-5.png)

   >[!NOTE]
   >
   >Vyn Redigera sidlayout har inte uppdaterats i [!DNL Salesforce Lightning] ännu.

1. Välj **[!UICONTROL Fields]** i konsolen. Sök efter MSC i Snabbsökning. Alla nedtonade fält har lagts till i sidlayouten. Du måste ta bort dem.

   ![](assets/uninstall-salesforce-lightning-customization-package-6.png)

   >[!NOTE]
   >
   >Om inget av fälten är nedtonat betyder det att du inte har lagt till dem i sidlayouten. Du kan hoppa över det här avsnittet.

1. Bläddra till det avsnitt som innehåller dina [!DNL Sales Connect] anpassade fält.

   ![](assets/uninstall-salesforce-lightning-customization-package-7.png)

1. Det finns 10 typer av MSC-fält som kan läggas till i det här avsnittet. Ta bort alla fält som du har lagt till eller ta bort hela avsnittet.

1. Klicka på **[!UICONTROL Quick Save]** när du är klar.

   ![](assets/uninstall-salesforce-lightning-customization-package-8.png)

## Ta bort [!DNL Sales Connect]-knappar från sidlayouter {#remove-sales-connect-buttons-from-page-layouts}

1. Välj **[!UICONTROL Buttons]** i konsolen (steg 4 ovan). Sök i &quot;MSC.&quot; Alla nedtonade knappar har lagts till i det anpassade knappavsnittet. Du måste ta bort dem.

   ![](assets/uninstall-salesforce-lightning-customization-package-9.png)

   >[!NOTE]
   >
   >Om ingen av knapparna är nedtonad betyder det att du inte har lagt till dem. Du kan hoppa över det här avsnittet.

1. Dra och släpp MSC-knapparna från avsnittet [!UICONTROL Custom Buttons] till konsolen.

   ![](assets/uninstall-salesforce-lightning-customization-package-10.png)

1. Klicka på **[!UICONTROL Quick Save]** när du är klar.

   ![](assets/uninstall-salesforce-lightning-customization-package-11.png)

## Ta bort [!DNL Sales Connect] fält från avsnittet [!UICONTROL Activity History] {#remove-sales-connect-fields-from-activity-history-section}

1. Bläddra till sidans nedre del till det [!UICONTROL Activity History] relaterade listavsnittet och klicka på ikonen för skiftnyckel.

   ![](assets/uninstall-salesforce-lightning-customization-package-12.png)

1. Markera [!DNL Sales Connect]-fälten i området [!UICONTROL Selected Fields] och klicka på pilen [!UICONTROL Remove]. Klicka på **[!UICONTROL OK]** när du är klar.

   ![](assets/uninstall-salesforce-lightning-customization-package-13.png)

   >[!NOTE]
   >
   >Förkortningen MSE _är_ [!DNL Sales Connect]. Det är bara det föregående namnet&quot;Marketo Sales Engage&quot;.

1. Klicka på **[!UICONTROL Save]** när du är klar med sidan Leads.

## Ta bort [!DNL Sales Connect] gruppåtgärdsknappar från leadlistvyn {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. Klicka på kugghjulsikonen i [!DNL Salesforce Lightning] och välj **[!UICONTROL Setup]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-14.png)

1. Klicka på **[!UICONTROL Object Manager]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-15.png)

1. Rulla ned till och välj **[!UICONTROL Lead]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-16.png)

1. Klicka på **[!UICONTROL Search Layouts]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-17.png)

1. Klicka på pilen bredvid [!UICONTROL List View] och välj **[!UICONTROL Edit]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-18.png)

1. Välj **[!UICONTROL Add to MSC Campaign]**, **[!UICONTROL Email with MSC]** och **[!UICONTROL Push to MSC]** och klicka på pilen [!UICONTROL Remove]. Klicka sedan på **[!UICONTROL Save]**.

   ![](assets/uninstall-salesforce-lightning-customization-package-19.png)

Du bör inte längre se knapparna i leadlistevyn.

## Ta bort MSC-konfiguration för kontakter {#remove-msc-configuration-for-contacts}

1. Klicka på kugghjulsikonen i [!DNL Salesforce Lightning] och välj **[!UICONTROL Setup]**.

1. Klicka på **[!UICONTROL Object Manager]**.

1. Rulla ned till och välj **[!UICONTROL Contact]**.

1. Klicka på **[!UICONTROL Page Layouts]**.

1. Klicka på **[!UICONTROL Contact Layout]**.

1. Upprepa steg från alla tre avsnitten.

## Ta bort MSC-konfiguration för affärsmöjlighet {#remove-msc-configuration-for-opportunity}

1. Klicka på kugghjulsikonen i [!DNL Salesforce Lightning] och välj **[!UICONTROL Setup]**.

1. Klicka på **[!UICONTROL Object Manager]**.

1. Rulla ned till och välj **[!UICONTROL Opportunity]**.

1. Klicka på **[!UICONTROL Page Layouts]**.

1. Klicka på **[!UICONTROL Opportunity Layout]**.

Affärsmöjlighetsvyn har bara en knapp -&quot;Skicka MSE-e-post&quot; och följande fält:

![](assets/uninstall-salesforce-lightning-customization-package-20.png)

## Ta bort MSC-konfiguration för konto {#remove-msc-configuration-for-account}

1. Klicka på kugghjulsikonen i [!DNL Salesforce Lightning] och välj **[!UICONTROL Setup]**.

1. Klicka på **[!UICONTROL Object Manager]**.

1. Rulla ned till och välj **[!UICONTROL Account]**.

1. Klicka på **[!UICONTROL Page Layouts]**.

1. Klicka på **[!UICONTROL Account Layout]**.

Kontovyn har bara en knapp -&quot;Skicka MSE-e-post&quot; och följande fält:

![](assets/uninstall-salesforce-lightning-customization-package-21.png)

## Ta bort Marketo Sales Outbox {#remove-marketo-sales-outbox}

1. I [!DNL Salesforce] klickar du på fliken **+** högst upp på skärmen.

1. Klicka på **[!UICONTROL Customize My Tabs]**.

1. Välj alternativet Marketo Sales Outbox till höger. Klicka på pilen [!UICONTROL Remove] och sedan på **[!UICONTROL Save]**.

## Ta bort [!DNL Sales Connect]-paket {#delete-sales-connect-package}

När du har tagit bort alla objekt från ditt [!DNL Salesforce]-konto följer du stegen nedan.

1. Klicka på kugghjulsikonen i [!DNL Salesforce Lightning] och välj **[!UICONTROL Setup]**.

1. Ange&quot;Apex Classes&quot; i rutan Snabbsökning.

1. Klicka på **[!UICONTROL Delete]** bredvid alla MarketoSalesConnectionCustomization- eller MarketoSalesEngageCustomization-poster i listan.

Allt är klart!

Här är en lista över alla objekt som behöver tas bort från din [!DNL Salesforce]-instans:

## Anpassningsinformation för [!DNL Sales Connect] {#sales-connect-customization-details}

<table>
 <tr>
  <th>Anpassade aktivitetsfält</th>
  <th>Beskrivning</th>
  <th>Typ</th>
  <th>Datatyp</th>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Call Local Presence ID]</td>
  <td>Som användare kan jag välja Lokal närvaro som alternativ när jag ringer samtal från MSC Phone. Inkommande samtal visar ett lokalt nummer för mottagaren</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Call Recording URL]</td>
  <td>Samtal kan spelas in och en länk för inspelningen loggas här </td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Campaign]</td>
  <td>Loggnamn för MSC-kampanjen som kontakten/leadet är på</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Campaign URL]</td>
  <td>Loggar URL till kampanjen som skapades i MSC. Om du klickar på detta öppnas kampanjen i MSC-webbappen</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Campaign Current Step]</td>
  <td>Om en kontakt/lead finns i en kampanj loggas namnet på steget som användaren är på</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Attachment Viewed]</td>
  <td>Loggar data när ett e-postmeddelande skickas med en bifogad fil som visas av mottagaren</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Clicked]</td>
  <td>Loggar en bock när mottagaren klickar på en länk i e-postmeddelandet</td>
  <td>Aktivitet</td>
  <td>Kryssruta</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Replied]</td>
  <td>Loggar en bock när mottagaren svarar på e-postmeddelandet</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Status]</td>
  <td>Visar om ett e-postmeddelande skickas/håller på att skickas/studsas (spårning av studsade e-postmeddelanden beror på vilken leveranskanal som används)</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Template]</td>
  <td>Loggnamn för MSC-mallen som användes i e-postmeddelandet som skickades till leadet/kontakten</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Template URL]</td>
  <td>Loggar URL till mallen som skapades i MSC. Om du klickar på det här öppnas mallen i MSC-webbprogrammet</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email URL]</td>
  <td>Om du klickar på den här URL:en öppnas kommandocentralen i MSC och historikfliken med personinformationsvyn öppnas där användaren kan se det skickade e-postmeddelandet</td>
  <td>Aktivitet</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>[!UICONTROL MSC Email Viewed]</td>
  <td>Loggar en bock när mottagaren visar ett e-postmeddelande</td>
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
  <td>MSC - Senaste marknadsföringsåtagande</td>
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
  <td>Beskrivning av ärendet</td>
  <td>
  <p>Konto
  <p>Kontakt
  <p>Lead
  <p>Möjligheter</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - senaste marknadsföringsengagemanget Source</td>
  <td>Source för marknadsföringsinsatser</td>
  <td>
  <p>Konto
  <p>Kontakt
  <p>Lead
  <p>Möjligheter</td>
  <td>Text</td>
 </tr>
 <tr>
  <td>MSC - Typ av senaste marknadsföringsåtagande</td>
  <td>Typ av engagemang (t.ex. webbaktivitet)</td>
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
  <td>Avanmäl dig</td>
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
  <td>[!UICONTROL Send MSC Email]</td>
  <td>Skicka e-post från [!DNL Salesforce]</td>
  <td>
  <p>Konto
  <p>Kontakt
  <p>Lead
  <p>Möjligheter</td>
 </tr>
 <tr>
  <td>[!UICONTROL Add to MSC Campaign]</td>
  <td>Lägg till i MSC-kampanjer från [!DNL Salesforce]</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Push to MSC]</td>
  <td>Skicka kontakt från [!DNL Salesforce] till MSC</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Call with MSC]</td>
  <td>Ring säljsamtal från [!DNL Salesforce]</td>
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
  <td>[!UICONTROL Add to MSC Campaign]</td>
  <td>Lägg till i MSC-kampanjer från [!DNL Salesforce]</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Push to MSC]</td>
  <td>Skicka kontakt från [!DNL Salesforce] till MSC</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email with MSC]</td>
  <td>E-post med MSC från [!DNL Salesforce]</td>
  <td>
  <p>Kontakt
  <p>Lead</td>
 </tr>
</table>
