---
description: Dialogrutor - Marketo Docs - produktdokumentation
title: Dialogrutor
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
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

Det finns flera attribut att välja bland. I det här exemplet väljer vi Lead State _is_ California and Company Size _is greater than_ 50.

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
>Om du använder en asterisk fungerar det som ett jokertecken för&quot;catch all&quot;. `https://*.website.com` placerar dialogrutan på alla sidor på webbplatsen, inklusive underdomäner (t.ex.: support.website.com). Och `https://website.com/folder/*` placerar dialogrutan på alla HTML-sidor i efterföljande mapp (t.ex.: Låt oss i det här fallet säga att mappen är &quot;sport&quot;, så: website.com/sports/baseball.html, website.com/sports/football.html osv.).
