---
description: Syncing Call and Call Key Messages - Marketo Docs - produktdokumentation
title: Synkronisera samtal och ringa nyckelmeddelanden
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Synkronisera samtal och ringa nyckelmeddelanden {#syncing-call-and-call-key-messages}

Anrop och anrop av nyckelmeddelandeobjekt i Veeva CRM synkroniseras som standard till Marketo Engage. Marketo synkroniserar data som är upp till sex månader gamla, baserat på Call Created Date.

>[!NOTE]
>
>Marketo sparar samtalsdata upp till sex månader från datumet för samtalet.

**Vilka utlösare/filter gäller meddelandet Ring upp och ringa upp nyckel?**

Utlösare:

* Tillagd till samtal
* Borttagen från samtal
* Tillagd till att anropa nyckelmeddelande
* Borttagen från anropsnyckelmeddelande
* Uppdaterat samtal
* Uppdaterat meddelande om samtalsnyckel

Filter:

* Har samtal
* Har meddelande om anropsnyckel

Följande fält för meddelandena Call and Call Key synkroniseras och kan användas som begränsningar och utlösare.

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        Objekt
      </th>
      <th>
        Fältetikett
      </th>
      <th>
        Beskrivning
      </th>
      <th>
        Fältnamn
      </th>
      <th>
        Datatyp
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Utlysning</td>
      <td>Redovisare</td>
      <td>Sök efter kontot som samtalet är kopplat till.</td>
      <td>Account_vod__c</td>
      <td>Uppslag (konto)</td>
    </tr>
    <tr>
      <td>Utlysning</td>
      <td>Samtalstyp</td>
      <td>Typ av samtal som underhålls av systemet baserat på typ och innehåll av samtalet. Detta fält används för rapportering. Giltiga värden är: Endast detalj, Detalj med exempel, Gruppdetalj, Gruppdetalj med Exempel, Endast exempel. Dessa värden bör inte ändras, men översättningarna för dessa plocklistor kan ändras. Deltagare har samma anropstyp som huvudanropet. För ett gruppsamtal med 3 proffs har alla fyra posterna anropstypen "Group Detail"</td>
      <td>Call_Type_vod__c</td>
      <td>Picklist</td>
    </tr>
    <tr>
     <td>Utlysning</td>
      <td>Kontakt</td>
      <td>Sök efter den kontakt (om någon) som samtalet är kopplat till.</td>
      <td>Contact_vod__c</td>
      <td>Uppslag (kontakt)</td>
    </tr>
    <tr>
      <td>Utlysning</td>
      <td>Datum</td>
      <td>Datum för samtalet när det sparades eller skickades för första gången. Det här fältet ställs in via en utlösare på aktuellt datum om varken datum- eller datetime-fältet anges.</td>
      <td>Call_Date_vod__c</td>
      <td>Datum</td>
    </tr>
    <tr>
      <td>Utlysning</td>
      <td>Är föräldrasamtalet?</td>
      <td>Formelfält som avgör om samtalsposten är överordnad samtalet eller en deltagarsamtalspost. 1 anger att posten är Parent Call. 0 anger att det är ett Deltagarsamtal.</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>Formel (tal)</td>
    </tr>
    <tr>
      <td>Utlysning</td>
      <td>Status</td>
      <td>Status för samtalet - planerad, sparad eller skickad. Använd översättningsworkbench för att ändra visningsvärdena. Utlösarna för anropet tittar i det här fältet för att se om anropet är låst (skickat). Värdet anges för användaren när knappen Spara eller Skicka trycks ned.</td>
      <td>Status_vod__c</td>
      <td>Picklist</td>
    </tr>
    <tr>
      <td>Utlysning</td>
      <td>Posttyp</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Posttyp</td>
    </tr>
    <tr>
      <td>Anropa nyckelmeddelande</td>
      <td>Utlysning</td>
      <td>Uppslag till samtalet. Varje nyckelmeddelande är associerat med ett samtal.</td>
      <td>Call2_vod__c</td>
      <td>Överordnad-detail(call)</td>
    </tr>
    <tr>
      <td>Anropa nyckelmeddelande</td>
      <td>Kategori</td>
      <td>Spelar in meddelandekategorin för meddelandet. Används främst för rapportering.</td>
      <td>Category_vod__c</td>
      <td>Picklist</td>
    </tr>
    <tr>
      <td>Anropa nyckelmeddelande</td>
      <td>CLM-presentationsnamn</td>
      <td>CLM-presentationsnamn med stämplar</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>Text (80)</td>
    </tr>
    <tr>
      <td>Anropa nyckelmeddelande</td>
      <td>Namn på nyckelmeddelande</td>
      <td>Namn på stämplat nyckelmeddelande</td>
      <td>Key_Message_Name_vod__c</td>
      <td>Text (80)</td>
    </tr>
    <tr>
      <td>Anropa nyckelmeddelande</td>
      <td>Produktnamn</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>Formel (text)</td>
    </tr>
    <tr>
      <td>Anropa nyckelmeddelande</td>
      <td>Reaktion</a>
      </td>
      <td>Plocklista för reaktion på meddelandet. Redigera plocklistan för att ändra reaktionsvärdena.</td>
      <td>Reaction_vod__c</td>
      <td>Picklist</td>
    </tr>
  </tbody>
</table>
