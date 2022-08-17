---
description: Chatbot Behavior - Marketo Docs - produktdokumentation
title: Chatbot-beteende
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Chatbot-beteende {#chatbot-behavior}

Här följer olika möjliga scenarier som överträffar Chatbot förväntade beteende hos besökaren i var och en av dem.

<table>
  <tbody>
    <tr>
      <th>Förkortning</th>
      <th>Detaljer</th>
    </tr>
    <tr>
      <td>D1, D2, D3 osv.</td>
      <td>Representerar flera dialogrutor där D1 är en dialogruta</td>
    </tr>
    <tr>
      <td>P1, P2, P3 osv.</td>
      <td>Representerar dialogprioriteringar där P1 är den högsta prioriteten</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3 osv.</td>
      <td>Representerar flera webbsidor där WP1 är den första webbsidan</td>
    </tr>
    <tr>
      <td>V1, V2, V3 osv.</td>
      <td>Representerar flera besökare på webbsidan där V1 är besökare ett</td>
    </tr>
   </tbody>
</table>

## Scenarier {#scenarios}

<table>
  <tr>
      <th>Scenario</th>
      <th>Chatbot-beteende förväntades</th>
      <th>Serverdelsåtgärd</th>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1</p>
      </td>
      <td>
        <p>D1 kommer att matchas till V1 </p>
      </td>
      <td>Utlösarantalet för D1 ökas med 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 kommer att matchas till V1</p>
        <p>Efter uppdatering kommer D1 att matchas igen</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Efter uppdatering, ingen ändring av D1-utlösare eller antal engagemang</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte</p>
      </td>
      <td>D1 kommer att matchas till V1</td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Ingen ändring av antalet D1-ärenden</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1-klickningar på D1 och ger det första svaret</p>
      </td>
      <td>D1 kommer att matchas till V1</td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Antal engagemang för D1 ökas med 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1-klickningar på D1 och ger det första svaret</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 kommer att matchas till V1</p>
        <p>Efter uppdateringen fortsätter D1</p>
      </td>
      <td>
        <p>Utlösarantalet och engagemangsantalet för D1 ökas med 1</p>
        <p>Efter uppdatering ändras inte antalet</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickar på D1, aktiverar chattbot och slutför D1</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 kommer att matchas till V1</p>
        <p>Efter uppdatering kommer ingen dialogruta eller nästa dialogruta att öppnas för V1</p>
      </td>
      <td>
        <p>Utlösarantalet, antalet engagemang och antalet slutförda aktiviteter för D1 ökar med 1</p>
        <p>Efter uppdatering kommer ingen dialogruta eller nästa dialogruta att lösas</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är avsedd endast för WP1, WP2</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte </p>
        <p>V1-besök WP2</p>
      </td>
      <td>
        <p>Sidbesök WP1, D1 löses till V1</p>
        <p>Sidbesök WP2, D1 löses till V2</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>I WP2 ändras inte antalet utlösare för D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är avsedd endast för WP1, WP2</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 och aktiverade</p>
        <p>V1-besök WP2</p>
      </td>
      <td>
        <p>Sidbesök WP1, D1 löses till V1</p>
        <p>Sidbesök WP2, D1 löses till V1</p>
      </td>
      <td>
        <p>Utlösarantalet och engagemangsantalet för D1 ökas med 1</p>
        <p>I WP2 ändras inte antalet</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>D2 för endast WP2</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1-klickningar på D1 och ger det första svaret</p>
        <p>V1-besök WP2</p>
      </td>
      <td>
        <p>D1 kommer att lösas på WP1</p>
        <p>D1 fortsätter till V1 på WP2</p>
      </td>
      <td>
        <p>Utlösarantalet och engagemangsantalet för D1 ökas med 1</p>
        <p>Ingen ändring av D2-utlösare eller antal engagemang</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>D2 för endast WP2</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte </p>
        <p>V1-besök WP2</p>
      </td>
      <td>D1 kommer att lösas på WP1<br/>
      D2 löses på WP2</td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Utlösarantalet för D2 ökas med 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>D2 för endast WP2</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickar på D1 och slutför D1</p>
        <p>V1-besök WP2</p>
      </td>
      <td>D1 kommer att lösas vid WP1 och efter slutförandet<br/>D2 löses på WP2</td>
      <td>
        <p>Utlösarantalet, antalet engagemang och antalet slutförda aktiviteter för D1 ökar med 1</p>
        <p>Utlösarantalet för D2 ökas med 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>D2 för endast WP2</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickar på D1 och slutför D1</p>
        <p>V1-besök WP2</p>
        <p>V1-klick på D2 ger det första svaret </p>
      </td>
      <td>D1 kommer att lösas vid WP1 och efter slutförandet<br/>D2 löses på WP2</td>
      <td>
        <p>Utlösarantalet, antalet engagemang och antalet slutförda aktiviteter för D1 ökar med 1</p>
        <p>Utlösar- och engagemangssiffran för D2 ökas med 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte</p>
        <p>D1 är opublicerad</p>
      </td>
      <td>D1 kommer att matchas till V1</td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Ingen ändring av antalet D1-ärenden</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte</p>
        <p>D1 är opublicerad</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 löses till V1 för första gången</p>
        <p>Efter uppdatering kommer ingen dialogruta att lösas</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Ingen ändring av antalet D1-ärenden</p>
        <p>Efter uppdatering, ingen ändring av D1-utlösaren eller antalet engagemang</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 upptagen med D1 </p>
        <p>D1 är opublicerad</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 kommer att matchas till V1</p>
        <p>Efter uppdateringen fortsätter D1</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Antal D1-engagemang kommer att ökas med 1</p>
        <p>Efter uppdatering fortsätter D1 inte att ändras ytterligare för utlösar- eller engagemangssiffran</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte</p>
        <p>D1 publiceras med nya ändringar</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 löses till V1 för första gången</p>
        <p>Dialogrutan med nya ändringar kommer att stängas efter uppdateringen</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Efter uppdatering, som D1 med nya ändringar men ingen ytterligare ändring av utlösarantalet</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 är endast avsedd för WP1</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1-klick på D1 ger det första svaret</p>
        <p>D1 publiceras med nya ändringar</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 löses till V1 för första gången</p>
        <p>Dialogrutan med gamla ändringar fortsätter efter uppdateringen</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Antal engagemang för D1 ökas med 1 </p>
        <p>Efter uppdatering visas den gamla D1 så att ingen ändring görs för att aktivera antalet</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 riktad mot WP1 med 1 prioritet</p>
        <p>D2 för WP1 med 2 prioriteter</p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickade på D1 men svarade inte</p>
        <p>D1 är opublicerad</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 löses till V1 för första gången</p>
        <p>Efter uppdatering kommer D2 att matchas till V1</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Efter uppdatering kommer antalet utlösare för D2 att ökas med 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 riktad mot WP1 med 1 prioritet</p>
        <p>D2 för WP1 med 2 prioriteter </p>
        <p>V1-besök WP1 för första gången</p>
        <p>V1 klickar på D1 och slutför D1</p>
        <p>V1 uppdaterar WP1 och se D2<br/>V1 klickar på D2 och slutför D2</p>
        <p>Marknadsföraren gjorde ändringar i D1 och publicerade på nytt</p>
        <p>V1 uppdaterar WP1</p>
      </td>
      <td>
        <p>D1 löses till V1 för första gången</p>
        <p>Efter uppdatering kommer D2 att matchas till V1</p>
        <p>När D1 och D2 är klara, oavsett vilka ändringar eller ompublicerade D1, visas inte D2 igen till V1</p>
      </td>
      <td>
        <p>Utlösarantalet, antalet engagemang och antalet slutförda aktiviteter för D1 ökar med 1</p>
        <p>Uppdatera när D2 har slutförts, ingen åtgärd behöver vidtas</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 som mål för WP1 med utlösaren "Time on Site" på 30 sekunder</p>
        <p>V1-besök WP1</p>
      </td>
      <td>
        <p>D1 kommer att lösas men kommer inte att utlösas till V1</p>
        <p>Efter 30 sekunder visas/utlöses D1 till V1</p>
      </td>
      <td>Utlösarantalet för D1 ökas endast med 1 efter 30+ sekunder som använts på webbsidan</td>
    </tr>
    <tr>
      <td>
        <p>D1 som mål för WP1, WP2 med utlösaren "Time on page" på 30 sekunder</p>
        <p>V1-besök WP1, WP2</p>
      </td>
      <td>
        <p>D1 kommer att lösas men kommer inte att utlösas till V1</p>
        <p>Efter 30 sekunder visas/utlöses D1 till V1</p>
      </td>
      <td>Utlösarantalet för D1 ökas endast med 1 efter 30+ sekunder som använts på webbsidan</td>
    </tr>
    <tr>
      <td>
        <p>D1 som mål för WP1 med utlösaren för"rullningsprocent" på 50</p>
        <p>V1-besök WP1</p>
      </td>
      <td>
        <p>D1 kommer att lösas men kommer inte att utlösas till V1</p>
        <p>Efter 50 % rullning visas/utlöses D1 till V1</p>
      </td>
      <td>Utlösarantalet för D1 ökas endast med 1 efter 50 % rullning</td>
    </tr>
    <tr>
      <td>
        <p>D1 som mål för WP1 med 1 prioritet och händelseutlösaren"Time on page" på 30 sekunder</p>
        <p>D2 för WP1 med 2 prioriteter och händelsens"sidrullningsprocent" på 50</p>
        <p>V1-besök WP1, efter 10 sekunders V1-besök WP2, V1-besök WP1</p>
      </td>
      <td>
        <p>På WP1 kommer D1 att lösas men kommer inte att aktiveras till V1</p>
        <p>På WP2 kommer D2 att lösas men inte aktiveras till V1</p>
        <p>På WP1 löses D1 och efter 20 sekunder aktiveras D1 till V1</p>
      </td>
      <td>Utlösarantalet för D1 ökas endast med 1 efter 30 sekunder</td>
    </tr>
    <tr>
      <td>
        <p>D1 som mål för WP1 med utlösaren "Time on Site" på 1 minut</p>
        <p>V1 besöker WP1 i 1 minut och visas som D1, men engagerar inte</p>
        <p>V1 stänger WP1 och återgår till WP1 2 dagar senare</p>
      </td>
      <td>
        <p>D1 visas automatiskt som V1 eftersom de redan uppfyller utlösningskriterierna under föregående session</p>
        <p>Samma logik gäller för"Tid på sida" och"procentuell sidrullning"</p>
      </td>
      <td>
        <p>Utlösarantalet för D1 ökas med 1</p>
        <p>Efter retur behöver ingen åtgärd vidtas</p>
      </td>
    </tr>
  </tbody>
</table>
