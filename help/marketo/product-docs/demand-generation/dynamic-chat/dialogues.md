---
description: Dialogrutor - Marketo Docs - produktdokumentation
title: Dialogrutor
hide: true
hidefromtoc: true
source-git-commit: bea169db9e2dd12f95b2a19aa9f922819770fc95
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 0%

---

# Dialogrutor {#dialogues}

Dialogrutor är de enskilda chattkonversationer du kommer att skapa. Lär dig hur du anpassar dem visuellt, avgör vilka sidor de visas på och avgör vad som sägs samt vem som ser dem.

## Skapa en ny dialogruta {#create-a-new-dialogue}

1. Klicka på **Dialogrutor**.

   ![](assets/dialogues-1.png)

1. Klicka på knappen **Skapa ny**.

   ![](assets/dialogues-2.png)

1. Ange ett namn (beskrivningen är valfri), ange prioritetsnivå och klicka på **Spara**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>Prioritetsnivån avgör var dialogrutan visas i listan (t.ex.: prioritet = 1 betyder att den kommer att vara högst upp).

## Målgruppskriterier {#audience-criteria}

På samma sätt som med Marketo smarta listor kan du definiera målgruppen med hjälp av attribut för målgruppskriterier. Du kan rikta kända eller okända leads med hjälp av attribut för härledning, lead eller företag (eller en kombination av dessa).

**Kända leads**

Det finns _många_-attributkombinationer att välja mellan. I det här exemplet riktar vi oss till alla **kända leads** i Kalifornien som arbetar på ett företag med mer än 50 anställda.

1. Ta bort attributet **Leadtillstånd** och dra det åt höger.

   ![](assets/dialogues-4.png)

1. __ Isis är inställd som standard. I fältet Välj värden skriver du in CA (du kan också klicka på listrutan och välja från listan).

   ![](assets/dialogues-5.png)

1. Ta attributet **Företagsstorlek** och dra det till den plats där det står _dra och släpp ett attribut här_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >Du kan också välja ett attribut genom att klicka på dess **+**-ikon.

1. Klicka på operatorlistrutan och välj **Större än**.

   ![](assets/dialogues-7.png)

1. Skriv 50 och klicka någon annanstans på skärmen för att spara.

   ![](assets/dialogues-8.png)

**Anonyma leads**

Det finns ett enkelt sätt att specifikt rikta in leads som ännu inte finns i din databas. I det här exemplet riktar vi oss mot alla **anonyma leads** som finns i New York-området.

1. Ta tag i attributet **Lead Email** och dra det åt höger.

   ![](assets/dialogues-9.png)

1. Klicka på operatorlistrutan och välj **Är tom**.

   ![](assets/dialogues-10.png)

1. Ta attributet **Inced State** och dra det till den plats där det står _dra och släpp ett attribut här_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >FÖRKLARA INFERERAT.

1. __ Isis är inställd som standard. I fältet Välj värden skriver du NY (du kan också klicka på listrutan och välja från listan).

   ![](assets/dialogues-12.png)

## Lägg till grupper {#add-groups}

Du kan också gruppera attribut om du vill ha alla attribut tillsammans med &quot;något&quot; av andra.

SLUTFÖR DETTA

## Mål {#target}

Här anger du de URL:er som du vill att en viss dialogruta ska visas på.

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

VISA EXEMPEL NEDAN

## Rapporter {#reports}

Text
