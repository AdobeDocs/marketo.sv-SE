---
unique-page-id: 37357302
description: E-postkolumner och e-postsidlayout - Marketo Docs - Produktdokumentation
title: E-postkolumner och sidlayout för e-post
exl-id: 689220e1-5ace-4225-98ff-21afd97f071b
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# E-postkolumner och sidlayout för e-post {#email-columns-and-email-page-layout}

Du kan konfigurera alla tillgängliga kolumner så att de visas i e-postavsnittet i [!UICONTROL Command Center]. Konfigurationsinställningarna sparas för varje e-postundermapp (t.ex. [!UICONTROL Delivered], [!UICONTROL Failed], [!UICONTROL Scheduled]).

## E-postkolumner {#email-columns}

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><p>Kolumn</p></th>
   <th>Beskrivning</th>
  </tr>
  <tr>
   <td>[!UICONTROL Person]</td>
   <td>Namn och e-postadress för personen i [!DNL Sales Connect]. Om du klickar på det här fältet öppnas fliken Om i vyn Personinformation.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Name]</td>
   <td>Namn på personen i [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td>[!UICONTROL Address]</td>
   <td>Personens primära e-postadress i [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td>[!UICONTROL Campaign]</td>
   <td>Om e-postmeddelandet skickades som en del av en kampanj visas kampanjens namn. Om du klickar på det här fältet kommer du till inställningssidan för den kampanjen.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Template]</td>
   <td>Visar namnet på mallen (om e-postmeddelandet skickades med ett).</td>
  </tr>
  <tr>
   <td colspan="1">[!UICONTROL Subject]</td>
   <td colspan="1">E-postmeddelandets ämnesrad.</td>
  </tr>
  <tr>
   <td colspan="1">[!UICONTROL Groups]</td>
   <td colspan="1">Visar de grupper som e-postmottagaren tillhör.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Job Title]</td>
   <td>E-postmottagarens namn.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Company]</td>
   <td>E-postmottagarens företag.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Email Status]</td>
   <td>Status som e-postmeddelandet är i. Status: Utkast, Schemalagd, Pågår, Skräppost, Avbruten, Misslyckad, Skickad. Skickade e-postmeddelanden visar en aktivitetsström som visar hur många visningar, klickningar och svar som har gjorts i det e-postmeddelandet.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Date Created]</td>
   <td>Datum när e-postmeddelandet skapades.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Last Updated]</td>
   <td>Datum när e-postmeddelandet senast uppdaterades.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Delivery Channel]</td>
   <td>Namnet på den leveranskanal som användes för att skicka e-postmeddelandet.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Latest Activity]</td>
   <td>E-postmottagarens senaste engagemang (t.ex. visa, klicka eller svara).</td>
  </tr>
  <tr>
   <td>[!UICONTROL Date Sent]</td>
   <td>Det datum då e-postmeddelandet skickades.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Follow Up] Åtgärder</td>
   <td>Snabbåtgärdsknappar som kan användas för uppföljning via e-post, telefon, iMail eller uppgift.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Group Email]</td>
   <td>Visar en bock om e-postmeddelandet skickades som en del av ett gruppe-postmeddelande.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Task Due Date]</td>
   <td>Visar förfallodatumet för aktiviteter som är relaterade till e-postmeddelandet. Uppgifter kan relateras till ett e-postmeddelande genom att skapas från snabbåtgärdsknapparna i e-postlistan.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Email Action]</td>
   <td>Snabbåtgärdsknappar som kan användas för att utföra åtgärder i e-postmeddelandet. Beroende på status för e-postmeddelandet kan följande åtgärder vara tillgängliga: Arkiv, Slutfört, Ta bort, Försök skicka igen, Avarkivera.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Task Type]</td>
   <td>Visar uppgiftstypen för en aktivitet som är relaterad till e-postmeddelandet. Uppgifter kan relateras till ett e-postmeddelande genom att skapas från snabbåtgärdsknapparna i e-postlistan.</td>
  </tr>
  <tr>
   <td>[!UICONTROL Date Failed]</td>
   <td>Visar det datum då e-postmeddelandet misslyckades om e-postmeddelandet inte levererades.</td>
  </tr>
 </tbody>
</table>

## Inställningar för sidlayout för e-post {#email-page-layout-settings}

Du kan konfigurera layouten genom att följa dessa steg.

1. Gå till **[!UICONTROL Command Center]**.

   ![](assets/email-columns-and-email-grid-layout-1.png)

1. Markera avsnittet **[!UICONTROL Emails]**.

   ![](assets/email-columns-and-email-grid-layout-2.png)

1. Klicka på knappen Konfiguration. Dina alternativ är bland annat: välja hur många rader du vill ha, välja vilka fält du vill ska visas och välja om du vill att gruppmeddelanden ska samlas i ett enda objekt i rutnätet (eller om du vill att alla e-postmeddelanden som är en del av ett e-postrutnät ska visas som ett enda objekt).

   ![](assets/email-columns-and-email-grid-layout-3.png)

1. Klicka utanför konfigurationen när du är klar.
