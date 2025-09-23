---
unique-page-id: 11379928
description: Ändra detaljer i granskningsspår - Marketo Docs - produktdokumentation
title: Ändra detaljer i granskningsspår
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1902'
ht-degree: 0%

---

# Ändra detaljer i granskningsspår {#change-details-in-audit-trail}

Granskningsspårning ger en hel del insikt i vem som gör vad i din Marketo-prenumeration. Här är detaljerna.

## Resursgranskningsspår {#asset-audit-trail}

<table>
 <colgroup>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th colspan="1">Tillgång/typ</th>
   <th colspan="1">Åtgärd</th>
   <th colspan="1">Ändra information</th>
  </tr>
  <tr>
   <td rowspan="15"><strong>Standardprogram</strong><br><br><br><br><br><br><br><br><br><br><br></td>
   <td>Skapa</td>
   <td>Kanaltypen "kanaltyp"<br>eller<br>klonad från "programnamn"</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till arbetsytans"arbetsytans namn" <br>Plats"Kampanjmapp" eller"engagemangsprogram" <br>Klonat programnamn"nytt namn"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Redigera kanal</td>
   <td>Ny kanal,"nytt kanalnamn" Gammal kanal,"gammalt kanalnamn" </td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Lägg till token "token name"-värdet "token value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Redigera token "tokennamn" nytt värde "nytt värde" gammalt värde "gammalt värde"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Ta bort token "tokennamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Lägg till analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td><p>Redigera analysbeteendet"beteendenamn"</p><p>Gammalt beteendenamn</p></td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Ta bort analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Lägg till periodkostnadsvärdet "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Redigera periodkostnad Nytt kostnadsvärde "#", Ny programmånad "yyyy-mm", Gammalt kostnadsvärde "#", Gammal programmånad "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Radera periodkostnad. Värde "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td>Exportera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td rowspan="19"><strong>E-post</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td>
   <td>Skapa</td>
   <td>Skapad med mallen "mallnamn" <br> eller <br>klonad från "resursnamn"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Uppdaterat Från namn till Nytt från namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Uppdaterat Från e-post till newemail@name.com</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Uppdaterat"Svara till" till"newreplytoemail@name.com"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Uppdaterat"Ämne" till"ny ämnesrad"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Lagt till segmentering "segmentation_name"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Avlägsen segmentering</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Utdraget "snippet_name" har lagts till</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Borttaget fragment</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Redigerar pank e-post från mallen "template_name" (Obs! Detta händer idag om du redigerar koden direkt)</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning "new description" Gammal beskrivning "old description"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Redigera modulen <code>"&lt;module name&gt;" &lt;attribute&gt;</code> till "värde"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till Design Studio i mappen "foldername" <br>Namnet "name"<br>eller<br>Klonad till "Marketing Activities" i programmet "program name"<br>Namnet på den klonade mediefilen "name"</td>
  </tr>
  <tr>
   <td>Flytta</td>
   <td>Flyttad till Design Studio i mappen "mappnamn"<br>eller<br>Flyttad till "marknadsföringsaktiviteter" i programmet "programnamn"</td>
  </tr>
  <tr>
   <td>Godkänn</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Godkänn inte</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Utkast</td>
   <td>E-postmeddelandet har skrivits ut eftersom fragmentets kodavsnittsnamn godkändes<br>eller<br>E-postmeddelandet har skrivits eftersom mallens mallnamn godkändes</td>
  </tr>
   <td rowspan="17">E-postprogram</td>
   <td>Skapa</td>
   <td>Kanaltypen "kanaltyp"<br>eller<br>klonad från "programnamn"</td>
  </tr>
  <tr>
   <td colspan="1">Byt namn</td>
   <td colspan="1">Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till arbetsytans"arbetsytans namn" <br>Plats"Kampanjmapp eller engagemangsprogram" <br>Klonat programnamn"nytt namn"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Avbryt</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Redigera kanal</td>
   <td>New channel "new channel" Old channel "old channel"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Lägg till token "token name"-värdet "token value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Redigera token "token name" Nytt värde "new value" gammalt värde "old value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Ta bort token "tokennamn"</td>
  </tr>
  <tr>
   <td>Ändra programschema</td>
   <td>Ange att schemat ska börja på startdatum, starttid och sluta med slutdatum, sluttid</td>
  </tr>
  <tr>
   <td>Ändra programschema</td>
   <td>Schemat har ändrats till "nytt datum, ny tid"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Lägg till analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Redigera analysbeteendet "beteendenamn"<br>Gammalt beteende "beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Ta bort analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Lägg till periodkostnadsvärdet "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Redigera periodkostnad Nytt kostnadsvärde "#", Ny programmånad "yyyy-mm", Gammalt kostnadsvärde "#", Gammal programmånad "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Radera periodkostnad. Värde "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td rowspan="8">E-postmall</td>
   <td>Skapa</td>
   <td>Tom eller klonad från "mallnamn"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning,"ny beskrivning", föregående beskrivning"föregående beskrivning"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>HTML Editing</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonat till "mappnamn" <br> klonat resursnamn "namn"</td>
  </tr>
  <tr>
   <td>Godkänn</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Godkänn inte</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td rowspan="23">Engagement Program</td>
   <td>Skapa</td>
   <td>Kanaltypen "kanaltyp"<br> eller<br> klonad från "programnamn"</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till arbetsytans"arbetsytans namn" <br>Plats"Kampanjmapp eller engagemangsprogram" <br>Klonat programnamn"nytt namn"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Redigera kanal</td>
   <td>New channel "new channel" Old channel "old channel"</td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td><p>Lägg till ström</p><p>Namnge "name"-placering "#"</p></td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td><p>Redigera ström</p><p>Nytt strömnamn: "nytt namn" Gammalt strömnamn: "gammalt namn"</p><p>Ny placering: "new #" Gammal placering: "old #"</p></td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td>Ta bort strömmens namn</td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td>Lägg till innehåll<br>Namn på ström<br>Skriv "E-post" eller "Program"<br>Namn "E-postnamn" eller "programnamn"<br>Smart Campaign "namn på smart kampanj"</td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td>Aktivera innehåll<br>Strömnamnet"strömnamn"<br>Innehållsnamnet"e-postnamn" eller"programnamn"</td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td>Inaktivera innehåll<br>Strömnamnet "strömnamn"<br>Innehållsnamnet "e-postnamn" eller "programnamn"</td>
  </tr>
  <tr>
   <td>Ändra programström</td>
   <td>Ta bort innehåll<br>Strömnamnet "strömnamn"<br>Innehållsnamnet "e-postnamn" eller "programnamn"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Lägg till token "token name"-värdet "token value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Redigera token "token name" Nytt värde "new value" gammalt värde "old value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Ta bort token "tokennamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Lägg till analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Redigera analysbeteendet "beteendenamn"<br>Gammalt beteende "beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Ta bort analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Ändra programstatus. Nytt värde av/på Gammalt värde av/på</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Lägg till periodkostnadsvärdet "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Redigera periodkostnad Nytt kostnadsvärde "#", Ny programmånad "yyyy-mm", Gammalt kostnadsvärde "#", Gammal programmånad "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Radera periodkostnad. Värde "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td>Exportera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td rowspan="18">Event Program</td>
   <td>Skapa</td>
   <td>Kanaltypen "kanaltyp"<br>eller<br>klonad från "programnamn"</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till arbetsytans "arbetsytans namn" <br>Plats "kampanjmapp" eller "engagemangsprogram" <br>Klonat programnamn "nytt namn"</td>
  </tr>
  <tr>
   <td>Redigera kanal</td>
   <td>New channel "new channel" Old channel "old channel" </td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Lägg till token "token name"-värdet "token value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Redigera token "token name" Nytt värde "new value" gammalt värde "old value"</td>
  </tr>
  <tr>
   <td>Ändra programtoken</td>
   <td>Ta bort token "tokennamn"</td>
  </tr>
  <tr>
   <td>Ändra programschema</td>
   <td>Ange att schemat ska börja på startdatum, starttid och sluta med slutdatum, sluttid</td>
  </tr>
  <tr>
   <td>Ändra programschema</td>
   <td>Schemat har ändrats till "nytt datum, ny tid"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Lägg till analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Redigera analysbeteendet "beteendenamn"<br>Gammalt beteende "beteendenamn"</td>
  </tr>
  <tr>
   <td>Ändra programinställningar</td>
   <td>Ta bort analysbeteendet"beteendenamn"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Lägg till periodkostnadsvärdet "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Redigera periodkostnad Nytt kostnadsvärde "#", Ny programmånad "yyyy-mm", Gammalt kostnadsvärde "#", Gammal programmånad "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Radera periodkostnad. Värde "#" för programmånaden "yyyy-mm"</td>
  </tr>
  <tr>
   <td colspan="1">Ändra programinställningar</td>
   <td colspan="1">Deltagaren"partner_namn" har lagts till</td>
  </tr>
  <tr>
   <td>Exportera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td rowspan="5">Mappar</td>
   <td>Skapa</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Token "token_name", value "value" har lagts till</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Redigerat token "token_name" nytt värde "token_value" gammalt värde "old_token_value"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Token "token_name" har tagits bort</td>
  </tr>
  <tr>
   <td rowspan="8">Forms</td>
   <td>Skapa</td>
   <td>Kommer snart. Lär dig mer eller klonad från"formulärnamn"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning "new description" Gammal beskrivning "old description"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Redigerade formulärinställningar </td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Information om redigerade fält</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till Design Studio i mappen "foldername" <br>Namnet "name"<br>eller<br>Klonad till "Marketing Activities" i programmet "program name"<br>Namnet på den klonade mediefilen "name"</td>
  </tr>
  <tr>
   <td>Flytta</td>
   <td>Flyttad till Design Studio i mappen "mappnamn"<br>eller<br>Flyttad till "marknadsföringsaktiviteter" i programmet "programnamn"</td>
  </tr>
  <tr>
   <td>Forms</td>
   <td>Godkänn</td>
   <td>Används av # resurser </td>
  </tr>
  <tr>
   <td rowspan="9">Landningssida</td>
   <td>Skapa</td>
   <td>Skapad med mallen "mallnamn" <br> eller <br>klonad från "resursnamn"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning,"ny beskrivning" Föregående"föregående beskrivning"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Lagt till "Image", borttagen "Image", redigerad bildkomponent</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Lagt till "RTF", borttagen "RTF", redigerad RTF-komponent</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till "Design Studio" i mappen "foldername"<br>Klonat resursnamn "name"<br>Klonad resurs-URL "www.url.com"<br>eller<br>Klonad till "Marknadsföringsaktiviteter" i programmet "programnamn" <br>Klonat resursnamn "name"<br>Klonad resurs-URL "www.url.com"</td>
  </tr>
  <tr>
   <td>Flytta</td>
   <td>Flyttad till Design Studio i mappen "folder name" <br> eller <br> Flyttad till "Marketing tasks" i programmet "program name"</td>
  </tr>
  <tr>
   <td>Godkänn</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Utkast</td>
   <td>Landningssidan har skapats eftersom mallnamnet godkändes</td>
  </tr>
  <tr>
   <td>Godkänn inte</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td rowspan="8">Landningssidmall</td>
   <td>Skapa</td>
   <td><p>Tom<br>eller<br>klonad från "resursnamn"</p></td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning,"ny beskrivning", föregående beskrivning,"föregående beskrivning"</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonat till "mappnamn" <br>Namnet på den klonade resursen "namn"</td>
  </tr>
  <tr>
   <td>Exportera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Godkänn</td>
   <td>Används av # resurser </td>
  </tr>
  <tr>
   <td>Godkänn inte</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td rowspan="5">Lista (statisk)</td>
   <td>Skapa</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Exportera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till "Persondatabas" i mappen "mappnamn" <br>Namnet på den klonade resursen "namn"<br>eller<br>Klonad till "marknadsföringsaktiviteter" i programmet "programnamn"<br>Namnet på den klonade resursen "namn"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td rowspan="12">Smart Campaign</td>
   <td>Skapa</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Aktivera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Inaktivera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Avbryt</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Flytta</td>
   <td>Flyttad till Program i program <br>eller<br>Flyttad till Mappar i mappen "mappnamn"</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning,"ny beskrivning" Föregående"föregående beskrivning"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonat till Program i programmet Program <br>Klonat resursnamn <br>eller<br>Klonat till Mapp i mappnamn<br>Klonat resursnamn.</td>
  </tr>
  <tr>
   <td>Ändra konfigurationen för smartlist</td>
   <td>Visar en ögonblicksbild av det aktuella läget, inklusive namn och värden på filter och utlösare</td>
  </tr>
  <tr>
   <td>Ändra kampanjschema</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Ändra flödesstegåtgärd</td>
   <td>Visar en ögonblicksbild av det aktuella läget, inklusive namn och värden för varje flödessteg</td>
  </tr>
  <tr>
   <td rowspan="7">Smart List</td>
   <td>Skapa</td>
   <td>Klonad från "smart listnamn"</td>
  </tr>
  <tr>
   <td>Exportera</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning,"ny beskrivning" Föregående"föregående beskrivning"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonad till "Persondatabas" i mappen "mappnamn" <br>Namnet på den klonade resursen "namn"<br>eller<br>Klonad till "marknadsföringsaktiviteter" i programmet "programnamn" <br>Namnet på den klonade resursen "namn"</td>
  </tr>
  <tr>
   <td>Ändra konfigurationen för smartlist</td>
   <td>Visar en ögonblicksbild av det aktuella läget, inklusive namn och värden på filter och utlösare </td>
  </tr>
  <tr>
   <td rowspan="11">Fragment</td>
   <td>Skapa</td>
   <td><p>Tom<br>eller<br>klonad från "kodavsnittsnamn"</p></td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Lagt till segmentering "segmentation_name"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Avlägsen segmentering</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Redigerad</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Byt namn</td>
   <td>Nytt namn, tidigare namn</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Ny beskrivning,"ny beskrivning" Föregående"föregående beskrivning"</td>
  </tr>
  <tr>
   <td>Klona</td>
   <td>Klonat till "mappnamn" <br>Namnet "på det klonade fragmentet"</td>
  </tr>
  <tr>
   <td>Godkänn</td>
   <td>Används av # resurser</td>
  </tr>
  <tr>
   <td>Godkänn utan utkast</td>
   <td>Ej tillämpligt</td>
  </tr>
  <tr>
   <td>Godkänn inte</td>
   <td><p>Ej tillämpligt</p></td>
  </tr>
 </tbody>
</table>

## Granskningsspår för administratör {#admin-audit-trail}

<table>
 <colgroup>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th>Administratörsområde</th>
   <th>Åtgärd</th>
   <th>Ändra information</th>
  </tr>
  <tr>
   <td>IP-begränsningar</td>
   <td>Redigera</td>
   <td>Redigerade IP-begränsningar till följande: Tillåtet/blockerat "block", IP-adress "#", Inaktiverade IP-begränsningar ""</td>
  </tr>
  <tr>
   <td rowspan="2">Partition</td>
   <td>Skapa</td>
   <td>Partitionen har skapats med namnet partitionsnamn</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Partitionen "partitionsnamn" har tagits bort</td>
  </tr>
  <tr>
   <td>Lösenordsstyrka</td>
   <td>Redigera</td>
   <td>Lösenordsskydd har ändrats till mall: Standardsäkerhet, min längd: #, nedre övre: #, nummer: #, blandat skiftläge: # , förfallodatum : #, sessionstimeout: #</td>
  </tr>
  <tr>
   <td rowspan="3">Roll<br><br></td>
   <td>Skapa</td>
   <td>Roll skapad med rollnamn (Obs! Om du behöver information om behörigheter som lagts till kontaktar du support) - <br>visar en ögonblicksbild av behörigheter som tilldelats rollen</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Rollnamnet har tagits bort</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Roll redigerad från "tidigare namn" till "nytt namn" (Obs! Om du behöver information om redigerade behörigheter kontaktar du support) - <br>visar en ögonblicksbild av behörigheter som tilldelats rollen<br></td>
  </tr>
  <tr>
   <td>Smartlist Report</td>
   <td>Redigera</td>
   <td>SmarList har redigerats för inloggning för hämtning: "true or false"</td>
  </tr>
  <tr>
   <td rowspan="7">Användare<br><br><br><br></td>
   <td>Skapa (bjud in)</td>
   <td>Användare inbjuden med: E-postadress, Namn för- och efternamn, Åtkomst förfaller tom eller med ett datum, API-användare sant eller falskt - <br>visar ögonblicksbilder av roller och arbetsytor som tilldelats användaren</td>
  </tr>
  <tr>
   <td colspan="1">Ta bort</td>
   <td colspan="1">"user name" user deleted</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Användaren har bytt namn från "gammalt namn" till "nytt namn" med e-postadress: "email", apiUser: "true or false" åtkomst förfaller: "blank or with a date"</td>
  </tr>
  <tr>
   <td>Redigera</td>
   <td>Användaren har redigerats för e-post: "email", apiUser: "true or false", åtkomsten upphör: "blank or with a date"</td>
  </tr>
  <tr>
   <td colspan="1">Redigera</td>
   <td colspan="1">Visar en ögonblicksbild av det aktuella läget, inklusive roller och arbetsytor som tilldelats användaren</td>
  </tr>
  <tr>
   <td>Problem</td>
   <td>Kalenderlicens utfärdad till e-post: "användarens e-postadress", namn: "användarens namn"</td>
  </tr>
  <tr>
   <td>Återställ</td>
   <td>Lösenordsåterställning för namnet"name" och e-post"email"</td>
  </tr>
  <tr>
   <td rowspan="2">Workspace</td>
   <td>Skapa</td>
   <td>Workspace har skapats med namnet "workspace name"</td>
  </tr>
  <tr>
   <td>Ta bort</td>
   <td>Arbetsytans namn har tagits bort</td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Filtrerar i granskningsspår](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
