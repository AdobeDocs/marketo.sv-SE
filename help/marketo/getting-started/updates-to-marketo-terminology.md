---
unique-page-id: 11387674
description: Uppdateringar av Marketo Terminology - Marketo Docs - produktdokumentation
hide: true
hidefromtoc: true
title: Uppdateringar av Marketo Terminologi
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Uppdateringar av Marketo Terminologi {#updates-to-marketo-terminology}

Vi gör några ändringar i vår plattform, vilket kommer att påverka vad vissa saker kallas. Om du har en ny Marketo-instans från mars 2016, eller om ditt företag förnyades efter juli 2016, kanske du ser den nya terminologin nu.

Även om du kan se olika terminologi i Marketo-dokumentationen, kan du vara säker på att alla artiklar snart kommer att uppdateras för att återspegla dessa ändringar. Alla instruktioner är desamma.

Så vad har ändrats?

## Lead is Now Person {#lead-is-now-person}

Den största förändringen är namnbytet av lead/leads till person/personer.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Gammal</strong></td> 
   <td><strong>Nytt</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

I vissa fall tas ordet&quot;Lead&quot; helt enkelt bort.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Gammal</strong></td> 
   <td><strong>Nytt</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Lead och person **är samma sak**.

## Tokens {#tokens}

Tokens med ordet lead i dem **ändras inte**. Vi ber om ursäkt för all förvirring. Om du ändrar alla token så att de matchar den nya terminologin bryts en hel del tokens som används för närvarande. Du kommer fortfarande att se variabler som `{{lead.First Name}}`. Det finns inga personspecifika tokens.

>[!NOTE]
>
>Det finns *en*-token med namnet &quot;Person Notes&quot;, men den variabeln fanns alltid där. Det används vanligtvis för ett beskrivningsfält i CRM, om det är något.

## Fälthantering {#field-management}

Fält som innehåller termen Lead har ersatts med Person eller ordet Lead har tagits bort. Ett anmärkningsvärt undantag är dock fältet&quot;Leadägare&quot;. Det kallas nu&quot;försäljningsägare&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Gammal</strong></td> 
   <td><strong>Nytt</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>En fullständig lista över fältnamn som påverkas finns i [supportartikeln](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## Real-Time Personalization (RTP) är nu Web Personalization {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Gammal</strong></td> 
   <td><strong>Nytt</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Förutom namnändringen består den nu av fyra separata program:

| **[Personalization för webben](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Har egen panel på hemskärmen |
|---|---|
| **[Kontobaserad webbmarknadsföring](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Tillgängligt via Web Personalization |
| **[Anpassad återmarknadsföring](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Tillgängligt via Web Personalization |
| **[Prediktivt innehåll](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Har egen panel på hemskärmen |

>[!NOTE]
>
>De rutor som visas på startskärmen motsvarar de moduler som köpts.

Tack för ditt tålamod under den här uppdateringen.
