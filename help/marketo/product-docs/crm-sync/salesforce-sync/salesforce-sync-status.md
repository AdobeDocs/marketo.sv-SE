---
description: Salesforce Sync Status - Marketo Docs - Produktdokumentation
title: Status för Salesforce-synkronisering
translation-type: tm+mt
source-git-commit: 98af67caaf485535ba2177aa661a503990e8698d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---


# Salesforce-synkroniseringsstatus {#salesforce-sync-status}

Använd kontrollpanelen Synkroniseringsstatus för att visa synkroniseringsstatus som en del av synkroniseringsstegen och dess status.

Synkroniseringsstegen återspeglar push- eller pull-åtgärder för varje objekttyp för objektschemat och själva data. Statistik täcker nya poster, uppdateringar, borttagningar och antalet misslyckade under synkroniseringen. Användare kan filtrera efter datum, åtgärdstyp eller objekttyp. Kontrollpanelen Synkroniseringsstatus visar status för synkroniseringscykler de senaste fem dagarna.

>[!NOTE]
>
>Administratörsbehörigheter krävs

## Visa synkroniseringsstatus {#view-sync-status}

1. Klicka på **Admin**.

   ![](assets/salesforce-sync-status-1.png)

1. Klicka på Salesforce under Integrering och sedan på fliken Synkroniseringsstatus.

   ![](assets/salesforce-sync-status-2.png)

Statistik sorteras som standard efter den senast startade. Du kan sortera efter Början eller Avslutad den (från senaste till äldsta) genom att klicka på sorteringsikonen.

![](assets/salesforce-sync-status-3.png)

## Filtersynkroniseringsstatus {#filter-sync-status}

1. Om du vill filtrera data klickar du på filterikonen längst till höger på sidan.

   ![](assets/salesforce-sync-status-4.png)

1. Välj datum- och tidsintervall och klicka sedan på listrutorna för att filtrera efter objekttyp, Åtgärdstyp och/eller Statustyp.

   ![](assets/salesforce-sync-status-5.png)

1. Klicka på **Använd**.

   ![](assets/salesforce-sync-status-6.png)

**Valfritt steg**: Om du vill exportera synkroniseringsfel klickar du på  **Exportera**. Data exporteras som en CSV-fil.

![](assets/salesforce-sync-status-7.png)

## Synkronisera statusfält {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Fält</th> 
   <th>Beskrivning</th> 
   <th>Uppräkningsvärden</th> 
  </tr> 
  <tr> 
   <td colspan="1">Startades vid</td> 
   <td colspan="1">Startdatum/tid för synkroniseringscykeln (användarens tidszon)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Avslutad den</td> 
   <td colspan="1">Slutdatum/tid för synkroniseringscykeln (användarens tidszon)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objekt</td> 
   <td colspan="1">Objekttyp</td> 
   <td colspan="1">Kontakt, Person, Uppgift, Möjligheter, Lead, Övrigt enligt nedan</td> 
  </tr>  
  <tr> 
   <td colspan="1">Åtgärd</td> 
   <td colspan="1">Åtgärdstyp</td> 
   <td colspan="1">Åtgärdstyper nedan</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status</td> 
   <td colspan="1">Status för batchen</td> 
   <td colspan="1">Slutförd, Misslyckad, Ofullständig, Pågår, Rensad*</td> 
  </tr>
  <tr> 
   <td colspan="1">Nytt</td> 
   <td colspan="1">Antal nya poster</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Uppdaterat</td> 
   <td colspan="1">Antal uppdaterade poster</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Borttagen</td> 
   <td colspan="1">Antal borttagna poster</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Misslyckat objekt</td> 
   <td colspan="1">Antal poster vars synkronisering misslyckades</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Överhoppad</td> 
   <td colspan="1">Antal poster som hoppats över eftersom inga ändringar har gjorts i intressefält för synkroniseringen</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

*Data återgick till det tidigare integritetstillståndet efter ett fel i synkroniseringssteget.

## Objekttyp {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">Konto</td> 
  </tr>  
  <tr> 
   <td colspan="1">Kontotyp</td> 
  </tr> 
  <tr> 
   <td colspan="1">Anpassade objekt</td> 
  </tr>  
  <tr> 
   <td colspan="1">Campaign</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status för kampanjmedlem</td> 
  </tr>
  <tr> 
   <td colspan="1">Kontakt</td> 
  </tr>  
  <tr> 
   <td colspan="1">E-postmall</td> 
  </tr>  
  <tr> 
   <td colspan="1">Händelse</td> 
  </tr> 
  <tr> 
   <td colspan="1">Person (ansvarig)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Möjligheter</td> 
  </tr>  
  <tr> 
   <td colspan="1">Roll för säljprojektskontakt</td> 
  </tr>  
  <tr> 
   <td colspan="1">Uppgift</td> 
  </tr>  
  <tr> 
   <td colspan="1">Användare</td> 
  </tr>  
 </tbody> 
</table>

## Åtgärdstyp {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Åtgärdstyp</th> 
   <th>Hittade mot dessa objekt</th> 
   <th>Anmärkningar</th> 
   <th>Åtgärdstyp</th>
  </tr> 
  <tr> 
   <td colspan="1">Ingångslänk till Program</td> 
   <td colspan="1">Campaign</td> 
   <td colspan="1">Länka kampanjer till program</td> 
   <td colspan="1">Uppdatera</td>
  </tr>  
  <tr> 
   <td colspan="1">Dragkonverteringar</td> 
   <td colspan="1">Person (ansvarig)*</td> 
   <td colspan="1">Dra in konverteringsåtgärder från SFDC till Marketo. Enheter (siffror) är leads som konverterar till kontakter</td> 
   <td colspan="1">Uppdatering, misslyckades eller hoppades över</td>
  </tr> 
  <tr> 
   <td colspan="1">Dragningar</td> 
   <td colspan="1">Kontakt, person (ansvarig), säljprojekt, kampanj, kampanjmedlemmar, säljprojektskontakt, anpassade objekt, kampanjer, status för kampanjmedlem, kontaktroll för säljprojekt</td> 
   <td colspan="1">Borttagna poster för SFDC som synkroniseras till Marketo</td> 
   <td colspan="1">Borttagen, misslyckades eller hoppades över</td>
  </tr>  
  <tr> 
   <td colspan="1">Hämta uppdateringar</td> 
   <td colspan="1">Aktivitet, person (ansvarig), person (ansvarig) kö, kontakt, händelse, möjlighet, konto, kontotyp, kampanjmedlemmar, anpassade objekt, kampanjer, kampanjmedlemmens status, händelser, personstatus, säljprojekt, säljprojektskontaktroll</td> 
   <td colspan="1">Uppdateringar eller nya poster i SFDC synkroniserade med Marketo, Pull Events as Activities</td> 
   <td colspan="1">Nytt, uppdaterat, misslyckat objekt eller överhoppat</td>
  </tr>  
  <tr> 
   <td colspan="1">Push new</td> 
   <td colspan="1">Uppgifter, e-postmallar</td> 
   <td colspan="1">Push-uppgifter (aktiviteter)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Push-uppdateringar</td> 
   <td colspan="1">Uppgifter, e-postmallar, person, kontakt, kampanjer</td> 
   <td colspan="1">Uppdateringar skickas till SFDC och tas även bort</td> 
   <td colspan="1">Uppdatering, misslyckades eller hoppades över</td>
  </tr>  
  <tr> 
   <td colspan="1">Synkroniseringsschema</td> 
   <td colspan="1">Kampanjmedlemmar, anpassade objekt, kampanjer, status för kampanjmedlem, uppgifter, person, säljprojekt, kontaktroll för säljprojekt, användare</td> 
   <td colspan="1">Synkroniserar metadata för olika objekt för att bestämma vilka nya fält som ska synkroniseras i nästa cykel</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Synkronisera med program</td> 
   <td colspan="1">Kampanjer</td> 
   <td colspan="1">Syncs Marketo-program med SFDC-kampanjer</td> 
   <td colspan="1">Nytt, Uppdateringar, Misslyckades eller Överhoppat</td>
  </tr> 
  <tr> 
   <td colspan="1">Uppdatera aktiviteter</td> 
   <td colspan="1">Uppgifter</td> 
   <td colspan="1">Dra in aktiviteter från Salesforce</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Uppdatera FKS</td> 
   <td colspan="1">Alla</td> 
   <td colspan="1">Uppdatera sekundärnyckel för alla objekt</td> 
   <td colspan="1">Ej tillämpligt</td>
  </tr>  
 </tbody> 
</table>

*Varumärkeskonfigurationen på prenumerationsnivå bestämmer etiketten - Lead eller Person i rapporten.
