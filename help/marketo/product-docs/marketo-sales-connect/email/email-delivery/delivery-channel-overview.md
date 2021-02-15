---
unique-page-id: 14352407
description: Översikt över leveranskanalen - Marketo Docs - Produktdokumentation
title: Översikt över leveranskanalen
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# Översikt över leveranskanalen {#delivery-channel-overview}

Vi kommer att bryta ned de tre olika kanalerna som du kan använda, hur du väljer dem, när du ska välja ut en av dem och nyanserna runt dem.

>[!NOTE]
>
>Den här informationen är bara relevant om du skickar e-post från [webbprogrammet](https://toutapp.com/login). Om du använder Sales Connect i Gmail eller Outlook levereras dina e-postmeddelanden via de e-postservrarna.

## MSC-e-postservrar (standard) {#msc-email-servers-default}

Som standard väljs den här metoden för leverans av dina e-postmeddelanden. MSC-e-postservrar är ett bra alternativ för användare som inte använder Gmail eller Outlook. Eftersom de är våra servrar har vi dessutom möjlighet att ta felmeddelanden om studsar eller misslyckade leveranser och visa upp dem för dig under&quot;Misslyckade leveranser&quot; på fliken Konversationer.

En annan fördel med att använda MSC-servrarna är att när mottagaren använder en [e-postadress](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/add-identity.md) ser han/hon e-postadressen till identiteten som du har skapat.

När du använder MSC-servrar kan mottagarna se taggen&quot;via toutapp.com&quot;. Det här är deras e-postklient som meddelar att e-postmeddelandet skickades med Sales Connect.

Mer information finns i den här [hjälpartikeln för Gmail](https://support.google.com/mail/answer/1311182?hl=en).

>[!NOTE]
>
>Våra MSC-servrar har ingen [DMARC-post](https://dmarc.org/) som är tillgänglig. De kan inte vitlistas på dina egna servrar.

## Gmail Server {#gmail-server}

Om ditt företags e-postleverantör är Gmail kan du använda ditt befintliga konto för att skicka dina Sales Connect-e-postmeddelanden. Detta är ett bra alternativ om du vill undvika informationen&quot;via toutapp.com&quot; och om du hellre vill förlita dig på företagets anseende och leveransförmåga. En annan fördel med att använda en Gmail-server är att allt du skickar ut från webbprogrammet automatiskt läggs till i Gmail-mappen som skickas.

Vi kan bara ansluta till ett enda Gmail-konto (en e-postadress) som kan leverera dina e-postmeddelanden om Sales Connect. Det innebär att om du använder flera e-postidentiteter visas bara adressen för det konto som vi är anslutna till när du tittar på informationen.

I webbprogrammet visas din identitet som du har skapat den (ovan). Om du skickar via Gmail-servrar visas adressen till det anslutna kontot.

>[!NOTE]
>
>Eftersom Sales Connect inte hanterar dina Gmail-servrar direkt kan vi inte spela in studsade e-posthändelser i webbprogrammet.

## Anpassad SMTP-server {#custom-smtp-server}

Betala för din egen server? Använda en Microsoft Exchange-miljö? Det här är ett alternativ för dig. Läs [de här instruktionerna](https://docs.marketo.com/x/zYTS) om hur du konfigurerar. Precis som Gmail-servrar spelar vi inte in studsade e-posthändelser i webbprogrammet eftersom Sales Connect inte hanterar servern direkt.
