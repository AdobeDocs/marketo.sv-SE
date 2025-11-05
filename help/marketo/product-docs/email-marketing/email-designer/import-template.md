---
solution: Marketo Engage
product: marketo
title: Import av mallar
description: Lär dig hur du importerar dina befintliga e-postmallar från den klassiska redigeraren till nya Email Designer.
level: Beginner, Intermediate
feature: Email Designer
badge: Beta
source-git-commit: 588ec23961df42de8a8c0aed919ba9a016b61f18
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Import av mallar {#template-import}

Importera enkelt dina befintliga e-postmallar från den klassiska redigeraren till nya Email Designer, bevara dina designer och snabba upp mallframtagningen med välbekanta, återanvändbara strukturer. Granska [bästa praxis](#best-practices) och läs mer om [begränsningar och åtgärder](#limitations-and-remedies).

>[!NOTE]
>
>De klassiska e-postmallarna har utvecklats med kostnadsfria HTML, så importören kanske inte alltid importerar alla komponenter perfekt. Granska de importerade mallarna för att se till att alla avsnitt är redigerbara och korrekt mappade. Om ett område inte kan markeras återskapar du det för bästa resultat.

## Importera en mall {#import-a-template}

1. Gå till **Design Studio**.

   ![](assets/import-template-1.png)

1. Klicka på **E-postmallar** och välj **E-postmallar (ny)**.

   ![](assets/import-template-2.png)

1. Klicka på **Skapa mall**.

   ![](assets/import-template-3.png)

1. Ange ett _namn_ och (valfritt) _Beskrivning_.

   ![](assets/import-template-4.png)

1. Klicka på fliken **Marketo-mallar** och välj bland de mallar som har skapats i den klassiska e-postredigeraren.

   ![](assets/import-template-5.png)

   >[!NOTE]
   >
   >Endast godkända mallar och mallar som har delats med den aktuella arbetsytan är tillgängliga för import.

1. Klicka på **Använd mallen**.

   ![](assets/import-template-6.png)

1. Den importerade mallen öppnas i e-post-Designer.

1. Granska komponenterna för korrekt konvertering och gör eventuella justeringar med Designer. När du är nöjd med mallen godkänner du den för användning i e-postmeddelanden.

## Skapa fragment {#create-fragments}

Det är en bra idé att skapa fragment av repeterbara avsnitt för senare bruk.

1. Klicka på knappen **..Mer** överst och välj **Spara som fragment**.

   ![](assets/import-template-7.png)

1. Markera en komponent eller struktur och klicka på **Skapa**.

   ![](assets/import-template-8.png)

1. Ange ett namn (och en valfri beskrivning) och klicka på **Spara**.

   ![](assets/import-template-9.png)

## Bästa praxis {#best-practices}

* De klassiska e-postmallarna har utvecklats med kostnadsfria HTML, så importören kanske inte alltid importerar alla komponenter perfekt. Granska de importerade mallarna för att se till att alla avsnitt är redigerbara och korrekt mappade. Om ett område inte kan markeras återskapar du det för bästa resultat.

* Efter importen kan du spara återanvändbara avsnitt som fragment och godkänna dem för användning av e-postförfattare. Använd varumärkesteman för att upprätthålla enhetlighet och regelefterlevnad.

* Du kan fortsätta använda QuickTime-skript och överväg att implementera om äldre fragment med en kombination av fragment och villkorligt innehåll för att få bättre flexibilitet och kontroll.

## Begränsningar och åtgärder {#limitations-and-remedies}

<table><thead>
  <tr>
    <th>Begränsning</th>
    <th>Orsak</th>
    <th>Åtgärda</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Variablerna som definieras i den klassiska e-postredigeraren är inte tillgängliga på e-postnivå.</td>
    <td>Variablerna var ursprungligen utformade för att förenkla e-postredigering när redigeraren ännu inte hade WYSIWYG-funktioner. I e-post-Designer kan användare uppnå liknande flexibilitet med de tillgängliga kontrollerna. Importören bibehåller strukturen och komponenterna i den befintliga mallen, vilket gör att du kan återskapa den effektivt i e-post-Designer.</td>
    <td>Användare bör kunna göra detta i Designer. <p>
    För moduler kan du spara olika segment som fragment. Godkända fragment kommer att vara tillgängliga för e-postnivå.</td>
  </tr>
  <tr>
    <td>Om HTML-källfilen innehåller kapslade block är de djupare lagren inte adresserbara i Designer.</td>
    <td>E-post-Designer stöder inte kapslade kommentarer.</td>
    <td>Även om Designer inte tillåter redigering av kapslade strukturer bör det återges korrekt. Testa mallen först.<p>
    Återskapa strukturen med stödraster.</td>
  </tr>
  <tr>
    <td>Ibland importeras knappar som enkla behållare med text inuti.</td>
    <td>Vissa implementeringsformat som använder HTML kan bli feltolkade vid import.</td>
    <td>Återskapa knappen i Designer.</td>
  </tr>
  <tr>
    <td>Knappar kan ibland vara för stora.</td>
    <td>Konflikt mellan CSS för Marketo-e-postmeddelanden och andra lågnivåelement (<code>&lt;span&gt;</code>)</td>
    <td>Prova att justera marginaler och utfyllnad för knappen i Designer.</td>
  </tr>
  <tr>
    <td>Punktpunkter stöds inte internt.</td>
    <td>Designer-e-postmeddelandet innehåller för närvarande inga punktlistor.</td>
    <td>Överväg att återskapa punkter med alternativa tekniker.</td>
  </tr>
  <tr>
    <td>Lodrät justering förvrängs om behållarens innehåll inte respekterar attributvärdet valign.</td>
    <td><code>valign</code> fungerar inte i behållare som definierats i mallen.</td>
    <td>Prova att justera marginaler och utfyllnad för knappen i e-postprogrammet Designer.</td>
  </tr>
  <tr>
    <td>Personalization Tokens (Mina token) på programnivå på mallnivå kan få valideringsfel.</td>
    <td>E-postmallar stöder inte token på programnivå.</td>
    <td>Ersätt dem med andra tokentyper i mallar och ersätt dem med Mina tokens inuti de enskilda e-postmeddelandena.</td>
  </tr>
  <tr>
    <td>Delningskomponenter kan inte markeras.</td>
    <td>Delningskomponenter omfattas inte av releasen.</td>
    <td>n/a</td>
  </tr>
  <tr>
    <td>Om den ursprungliga HTML har några oformaterade strukturer kommer de sannolikt att föras över.</td>
    <td>Problem med den ursprungliga HTML.</td>
    <td>Problemen måste åtgärdas före importen.</td>
  </tr>
  <tr>
    <td>För det importerade innehållet är användningen av förhandsgranskning av innehåll inte en tillförlitlig indikator.</td>
    <td>Designer förhandsvisningsfunktion stöder inte anpassade HTML.</td>
    <td>Vi rekommenderar att du testar din e-post med alternativet <b>Skicka korrektur</b> på skärmen <i>Simulera innehåll</i> .</td>
  </tr>
  <tr>
    <td>Fragment i den gamla mallen fungerar inte i e-post-Designer.</td>
    <td>Designer-e-postmeddelandet stöder inte fragment.</td>
    <td>Återskapa dina fragment som fragment kopplade till villkorsstyrt innehåll.</td>
  </tr>
</tbody></table>
