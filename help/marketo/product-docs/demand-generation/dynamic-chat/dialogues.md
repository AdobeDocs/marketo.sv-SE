---
description: Dialogrutor - Marketo Docs - produktdokumentation
title: Dialogrutor
hide: true
hidefromtoc: true
source-git-commit: d5c1c1d0ce2a521898eaa4f6610bf1ce04b4f66b
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Dialogrutor {#dialogues}

Dialogrutor är de enskilda chattkonversationer du kommer att skapa. Lär dig hur du anpassar dem visuellt, avgör vilka sidor de visas på och avgör vad som sägs samt vem som ser dem.

## Skapa en ny dialogruta {#create-a-new-dialogue}

1. Klicka på **Dialogrutor**.

PICC

1. Klicka på knappen **Skapa ny**.

PICC

1. Ange ett namn (beskrivningen är valfri), ange prioritetsnivå och klicka på **Spara**.

PICC

>[!NOTE]
>
>FÖRKLARA PRIORITETSNIVÅ

## Målgruppskriterier {#audience-criteria}

På samma sätt som med Marketo smarta listor kan du definiera målgruppen med hjälp av attribut för målgruppskriterier. Du kan rikta kända eller okända leads med hjälp av attribut för härledning, lead eller företag (eller en kombination av dessa).

Det finns _många_-attributkombinationer att välja mellan. I det här exemplet riktar vi oss mot alla kända leads i Kalifornien som arbetar på ett företag med över 50 anställda.

1. Hämta leadlägesattributet och dra det åt höger.

PICC

1. __ Isis är inställd som standard. I fältet Välj värden skriver du in CA (du kan också klicka på listrutan och välja från listan).

PICC

1. Ta attributet Företagsstorlek och dra det åt höger.

PICC

1. Klicka på operatorlistrutan och välj Större än.

PICC

1. Skriv 50 och klicka någon annanstans på skärmen för att spara.

PICC

HÄMTA ANON LEADS

Obs! Ange kanske hur inkommande arbete/visning av anon-användning är, lead-e-post är tom

## Lägg till grupper {#add-groups}

Du kan också gruppera attribut om du vill ha alla attribut tillsammans med &quot;något&quot; av andra.

SLUTFÖR DETTA

## Mål {#target}

Här anger du den eller de URL:er som du vill att en viss dialogruta ska visas på.

Godtagbara format:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>Om du använder en asterisk fungerar det som ett jokertecken för&quot;catch all&quot;. På så sätt placerar `https://*.website.com` dialogrutan på alla sidor på webbplatsen, inklusive underdomäner (t.ex.: `support.website.com`). Och `https://website.com/folder/*` placerar dialogrutan på alla HTML-sidor i efterföljande mapp (t.ex.: Låt oss i det här fallet säga att mappen är &quot;sport&quot;, så: website.com/sports/baseball.html, website.com/sports/football.html osv.).

## Stream Designer {#stream-designer}

Strömdesignern innehåller olika kort som du kan lägga till för att forma chattkonversationen.

<table>
 <tr>
  <td><strong>Meddelande</strong></td>
  <td>Använd när du vill göra en -programsats utan något svar (t.ex.: "Hej! Alla artiklar är 25 % rabatt idag med koden SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Fråga</strong></td>
  <td>Använd det här alternativet om du vill ställa en flervalsfråga, där du anger tillgängliga svar (t.ex.: Vilken typ av fordon är du intresserad av? Svar = SUV, Compact, Truck osv.).</td>
 </tr>
 <tr>
  <td><strong>Information Capture</strong></td>
  <td>Använd när du vill samla in information. De tre fälten som ska väljas är E-postadress, Telefonnummer och Text (som gör att besökaren kan skriva sitt eget meddelande).</td>
 </tr>
 <tr>
  <td><strong>Schemaläggare för avtalad tid</strong></td>
  <td>Ger besökaren en kalender med tillgängliga datum för att schemalägga en uppföljning. Kalendertillgängligheten återspeglar [nästa agent på rad](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).</td>
 </tr>
 <tr>
  <td><strong>Mål</strong></td>
  <td>Det här är det enda kortet som besökarna inte ser. Det är upp till dig att avgöra vid vilken punkt ett mål uppnås i den specifika chatten (t.ex.: om du vill samla in besökarens e-post, placerar du målkortet efter Info Capture i Stream).</td>
 </tr>
</table>

EVENTUELLT EGET AVSNITT

VISA EXEMPEL NEDAN