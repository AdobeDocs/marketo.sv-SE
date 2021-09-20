---
description: Dialogrutor - Marketo Docs - produktdokumentation
title: Dialogrutor
hide: true
hidefromtoc: true
source-git-commit: c6713c972603ab9528a66e908e47e4c187b86c0c
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Dialogrutor {#dialogues}

Dialogrutor är de specifika chattkonversationer du konfigurerar. De kan anpassas efter utseende, liksom vad som sägs och vem som ser det.

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

På samma sätt som med Marketo smarta listor kan du definiera målgruppen med hjälp av attribut för målgruppskriterier.

Det finns flera attribut att välja bland. I det här exemplet riktar vi oss mot alla kända leads i Kalifornien som arbetar på ett företag med över 50 anställda.

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

TABELL

Meddelande: Använd när du vill göra en -programsats utan något svar (t.ex.: &quot;Hej! Alla artiklar ger 25 % rabatt idag med kod SAVE25.&quot;)

Fråga: Använd det här alternativet om du vill ställa en flervalsfråga, där du anger tillgängliga svar (t.ex.: Vilken typ av fordon är du intresserad av? Svar = SUV, Compact, Truck osv.)

Information Capture: Använd när du vill samla in information. De tre fälten som ska väljas är E-postadress, Telefonnummer och Text (som gör att besökaren kan skriva sitt eget meddelande).

Schemaläggare för avtalad tid: Ger besökaren en kalender med tillgängliga datum för att schemalägga en uppföljning. Kalendertillgängligheten återspeglar [nästa agent på rad](help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).

Mål: Det här är det enda kortet som besökarna inte ser. Det är upp till dig att avgöra vid vilken punkt ett mål uppnås i den specifika chatten (t.ex.: om du vill samla in besökarens e-postadress placerar du målkortet efter Info Capture i Stream.)

EVENTUELLT EGET AVSNITT

VISA EXEMPEL NEDAN