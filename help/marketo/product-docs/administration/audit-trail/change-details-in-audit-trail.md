---
unique-page-id: 11379928
description: Ändra detaljer i granskningsspår - Marketo Docs - Produktdokumentation
title: Ändra detaljer i granskningsspår
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '1901'
ht-degree: 0%

---


# Ändra detaljer i granskningsspår {#change-details-in-audit-trail}

Granskningsspår ger en hel del insikt i vem som gör vad i er Marketo-prenumeration. Här är detaljerna.

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
   <td rowspan="15">Standardprogram<br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Skapa</td> 
   <td>Kanaltypen "kanaltyp"<br>eller<br>Klonad från "programnamn"</td> 
  </tr> 
  <tr> 
   <td>Byt namn</td> 
   <td>Nytt namn, tidigare namn</td> 
  </tr> 
  <tr> 
   <td>Klona</td> 
   <td>Klonad till arbetsytans "arbetsytans namn" <br>Plats "kampanjmapp" eller "engagemangsprogram" <br>Klonat programnamn "nytt namn"</td> 
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
   <td rowspan="18">E-post<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Skapa</td> 
   <td>Skapad med mallen "mallnamn" <br>eller <br>Klonad från "resursnamn"</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>Uppdaterat Från namn till Nytt från namn</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>Uppdaterat "Från e-post" till "<a href="http://docs.marketo.com/cdn-cgi/l/email-protection">[e-postskyddad]</a>"</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>Uppdaterat"Svara till" till"<a href="http://docs.marketo.com/cdn-cgi/l/email-protection">[e-postskyddad]</a>"</td> 
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
   <td>Redigerar skadat e-postmeddelande från mallen "template_name" (OBS: detta händer idag om du redigerar koden direkt)</td> 
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
   <td>Ny beskrivning,"ny beskrivning" Gammal beskrivning,"gammal beskrivning"</td> 
  </tr> 
  <tr> 
   <td>Klona</td> 
   <td>Klonad till "Design studio" i mappen "foldername" <br>Klonat resursnamn "name"<br>eller<br>Klonad till "Marketing Activities" i programmet "program name"<br>Klonat resursnamn "name"</td> 
  </tr> 
  <tr> 
   <td>Flytta</td> 
   <td>Flyttad till "Design studio" i mappen "folder name"<br>eller<br>Flyttad till "Marketing tasks" i programmet "program name"</td> 
  </tr> 
  <tr> 
   <td>Godkänn</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td>Avgodkänna</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td>Utkast</td> 
   <td>E-postmeddelandet har skrivits ut eftersom fragmentets"kodavsnittsnamn" godkändes<br>eller<br>E-postmeddelandet skapades eftersom mallens"mallnamn" godkändes</td> 
  </tr> 
  <tr> 
   <td rowspan="17">E-postprogram</td> 
   <td>Skapa</td> 
   <td>Kanaltypen "kanaltyp"<br>eller<br>Klonad från "programnamn"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Byt namn</td> 
   <td colspan="1">Nytt namn, tidigare namn</td> 
  </tr> 
  <tr> 
   <td>Klona</td> 
   <td>Klonad till arbetsytans "arbetsytans namn" <br>Plats "Kampanjmapp eller engagemangsprogram" <br>Klonat programnamn "nytt namn"</td> 
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
   <td>Ange att schemat ska börja på"startdatum, starttid" och sluta med"slutdatum, sluttid"</td> 
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
   <td>Redigera analysbeteendet"beteendenamn"<br>Gammalt beteende"beteendenamn"</td> 
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
   <td>Ny beskrivning, ny beskrivning, föregående beskrivning, föregående beskrivning</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>HTML-redigerad</td> 
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
   <td>Klonat till "mappnamn" <br> Namnet "namn" för den klonade resursen</td> 
  </tr> 
  <tr> 
   <td>Godkänn</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td>Avgodkänna</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td rowspan="23">Engagement Program</td> 
   <td>Skapa</td> 
   <td>Kanaltypen "kanaltyp"<br> eller<br> Klonad från "programnamn"</td> 
  </tr> 
  <tr> 
   <td>Byt namn</td> 
   <td>Nytt namn, tidigare namn</td> 
  </tr> 
  <tr> 
   <td>Klona</td> 
   <td>Klonad till arbetsytans "arbetsytans namn" <br>Plats "Kampanjmapp eller engagemangsprogram" <br>Klonat programnamn "nytt namn"</td> 
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
   <td><p>Redigera ström</p><p>Nytt strömnamn: "new name" Gammalt strömnamn: "gammalt namn"</p><p>Ny placering: "new #" Old Placement: "old #"</p></td> 
  </tr> 
  <tr> 
   <td>Ändra programström</td> 
   <td>Ta bort strömmens namn</td> 
  </tr> 
  <tr> 
   <td>Ändra programström</td> 
   <td>Lägg till innehåll<br>Steam name "stream name"<br>Skriv "Email" eller "Program"<br>Namn "email name" eller "program name"<br>Smart Campaign "smart campaign name"</td> 
  </tr> 
  <tr> 
   <td>Ändra programström</td> 
   <td>Aktivera innehåll<br>Strömnamn "strömnamn"<br>Innehållsnamn "e-postnamn" eller "programnamn"</td> 
  </tr> 
  <tr> 
   <td>Ändra programström</td> 
   <td>Inaktivera innehåll<br>Strömnamn "strömnamn"<br>Innehållsnamn "e-postnamn" eller "programnamn"</td> 
  </tr> 
  <tr> 
   <td>Ändra programström</td> 
   <td>Ta bort innehåll<br>Strömnamn "strömnamn"<br>Innehållsnamn "e-postnamn" eller "programnamn"</td> 
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
   <td>Redigera analysbeteendet"beteendenamn"<br>Gammalt beteende"beteendenamn"</td> 
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
   <td>Kanaltypen "kanaltyp"<br>eller<br>Klonad från "programnamn"</td> 
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
   <td>Ange att schemat ska börja på"startdatum, starttid" och sluta med"slutdatum, sluttid"</td> 
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
   <td>Redigera analysbeteendet"beteendenamn"<br>Gammalt beteende"beteendenamn"</td> 
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
   <td>Ny beskrivning,"ny beskrivning" Gammal beskrivning,"gammal beskrivning"</td> 
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
   <td>Klonad till "Design studio" i mappen "foldername" <br>Klonat resursnamn "name"<br>eller<br>Klonad till "Marketing Activities" i programmet "program name"<br>Klonat resursnamn "name"</td> 
  </tr> 
  <tr> 
   <td>Flytta</td> 
   <td>Flyttad till "Design studio" i mappen "folder name"<br>eller<br>Flyttad till "Marketing tasks" i programmet "program name"</td> 
  </tr> 
  <tr> 
   <td>Forms</td> 
   <td>Godkänn</td> 
   <td>Används av # resurser </td> 
  </tr> 
  <tr> 
   <td rowspan="9">Landningssida</td> 
   <td>Skapa</td> 
   <td>Skapad med mallen "mallnamn" <br>eller <br>Klonad från "resursnamn"</td> 
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
   <td>Klonad till"Design studio" i mappen"foldername"<br>Klonat resursnamn"name"<br>Klonad resurs-URL"www.url.com"<br>eller<br>Klonad till"Marknadsföringsaktiviteter" i programmet"programnamn" <br>Klonat resursnamn"namn"<br>Klonad resurs-URL"www.url.com"</td> 
  </tr> 
  <tr> 
   <td>Flytta</td> 
   <td>Flyttad till "Design studio" i mappen "mappnamn"<br> eller<br> Flyttad till "Marknadsföringsaktiviteter" i programmet "programnamn"</td> 
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
   <td>Avgodkänna</td> 
   <td>Ej tillämpligt</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Landningssidmall</td> 
   <td>Skapa</td> 
   <td><p>Tom<br>eller<br>Klonad från "resursnamn"</p></td> 
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
   <td>Klonat till "mappnamn" <br>Namnet "på den klonade resursen"</td> 
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
   <td>Avgodkänna</td> 
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
   <td>Klonad till "Persondatabas" i mappen "mappnamn" <br>Klonat resursnamn "namn"<br>eller<br>Klonad till "Marknadsföringsaktiviteter" i programmet "programnamn"<br>Klonat resursnamn "namn"</td> 
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
   <td>Flyttad till "Program" i programmet "programnamn"<br>eller<br>Flyttad till "Mappar" i mappen "mappnamn"</td> 
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
   <td>Klonat till Program i programmet "programnamn" <br>Klonat resursnamn "namn"<br>eller<br>Klonat till "Mapp" i mappen "mappnamn"<br>Klonat resursnamn "namn"</td> 
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
   <td>Klonat från "smart listnamn"</td> 
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
   <td>Klonad till "Persondatabas" i mappen "mappnamn" <br>Klonat resursnamn "namn"<br>eller<br>Klonad till "Marknadsföringsaktiviteter" i programmet "programnamn" <br>Klonat resursnamn "namn"</td> 
  </tr> 
  <tr> 
   <td>Ändra konfigurationen för smartlist</td> 
   <td>Visar en ögonblicksbild av det aktuella läget, inklusive namn och värden på filter och utlösare </td> 
  </tr> 
  <tr> 
   <td rowspan="11">Fragment</td> 
   <td>Skapa</td> 
   <td><p>Tom<br>eller<br>Klonad från "kodavsnittsnamn"</p></td> 
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
   <td>Klonat till "mappnamn" <br>Namnet på det klonade fragmentet "name"</td> 
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
   <td>Avgodkänna</td> 
   <td><p>Ej tillämpligt</p></td> 
  </tr> 
 </tbody> 
</table>

## Admin - Granskningsspår {#admin-audit-trail}

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
   <td>Redigerade IP-begränsningar till följande: Tillåtna/blockerade "block", IP-adress "#", inaktiverade IP-begränsningar ""</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Partition</td> 
   <td>Skapa</td> 
   <td>Partitionen har skapats med namnet "partitionsnamn"</td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>Partitionen "partitionsnamn" har tagits bort</td> 
  </tr> 
  <tr> 
   <td>Lösenordsstyrka</td> 
   <td>Redigera</td> 
   <td>Lösenordsskydd har ändrats till mall: Standardsäkerhet, min längd: #, lower-upper: #, nummer: #, blandat skiftläge: # , förfallodatum : #, timeout för session: #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">Roll<br><br></td> 
   <td>Skapa</td> 
   <td>Roll skapad med rollnamn (Obs! om du behöver information om behörigheter som lagts till, kontakta support) - <br>visar ögonblicksbilder av behörigheter som tilldelats rollen</td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>Rollnamnet har tagits bort</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>Roll redigerad från "tidigare namn" till "nytt namn" (Obs! om du behöver information om redigerade behörigheter, kontakta support) - <br>visar en ögonblicksbild av behörigheter som tilldelats rollen<br></td> 
  </tr> 
  <tr> 
   <td>Smartlist-rapport</td> 
   <td>Redigera</td> 
   <td>SmarList har redigerats för inloggning för nedladdning: "true or false"</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Användare<br><br><br><br></td> 
   <td>Skapa (bjud in)</td> 
   <td>Användare inbjuden med: E-postadress, namn för- och efternamn, åtkomst förfaller"tom eller med ett datum", API-användare"true eller false" - <br>visar en ögonblicksbild av roller och arbetsytor som tilldelats användaren</td> 
  </tr> 
  <tr> 
   <td colspan="1">Ta bort</td> 
   <td colspan="1">"user name" user deleted</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>Användaren har bytt namn från "gammalt namn" till "nytt namn" med e-post: "email", apiUser: "true or false"-åtkomst upphör: "blank or with a date"</td> 
  </tr> 
  <tr> 
   <td>Redigera</td> 
   <td>Användaren har redigerats för e-post: "email", apiUser: "true or false", åtkomst förfaller: "blank or with a date"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Redigera</td> 
   <td colspan="1">Visar en ögonblicksbild av det aktuella läget, inklusive roller och arbetsytor som tilldelats användaren</td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>Kalenderlicens utfärdad till e-post: "användarens e-postadress": "användarnamn"</td> 
  </tr> 
  <tr> 
   <td>Återställ</td> 
   <td>Lösenordsåterställning för namnet"name" och e-postadressen"email"</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Arbetsyta</td> 
   <td>Skapa</td> 
   <td>Arbetsytan har skapats med namnet "arbetsytans namn"</td> 
  </tr> 
  <tr> 
   <td>Ta bort</td> 
   <td>Arbetsytans namn har tagits bort</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [Filtrera i granskningsspår](filtering-in-audit-trail.md)

>



