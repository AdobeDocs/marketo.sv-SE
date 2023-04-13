---
unique-page-id: 4720710
description: Konfigurera SPF och DKIM för din e-postleverans - Marketo Docs - Produktdokumentation
title: Konfigurera SPF och DKIM för e-postleveransen
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: c69d04702a5191f2809cc308e48acfeab7edfc7f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Konfigurera SPF och DKIM för e-postleveransen {#set-up-spf-and-dkim-for-your-email-deliverability}

Ett snabbt sätt att förbättra e-postleveransen är att lägga till **SPF** (Sender Policy Framework) och **DKIM** (Domännycklar för identifierad e-post) till dina DNS-inställningar. Med det här tillägget i dina DNS-poster talar du om för mottagarna att du har auktoriserat Marketo att skicka e-post för din räkning. Utan den här ändringen har din e-postadress större chans att markeras som skräppost eftersom e-postadressen adresserades från din domän, men skickas från en IP-adress med en Marketo-domän.

>[!CAUTION]
>
>Du behöver din nätverksadministratör för att kunna göra den här ändringen i din DNS-post.

## Konfigurera SPF {#set-up-spf}

**Om du inte har någon SPF-post på din domän**

Be nätverksadministratören lägga till följande rad i DNS-posterna. Ersätt [domän] med webbplatsens huvuddomän (t.ex. &quot;company.com&quot;) och [corpIP] med IP-adressen till företagets e-postserver (t.ex. &quot;255.255.255.255&quot;). Om du skickar e-post från flera domäner via Marketo bör du lägga till detta i varje domän (på en rad).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Om du har en SPF-post på din domän**

Om du redan har en SPF-post i DNS-posten lägger du till följande i den:

include:mktomail.com

## Konfigurera DKIM {#set-up-dkim}

**Vad är DKIM? Varför vill jag konfigurera DKIM?**

DKIM är ett autentiseringsprotokoll som används av e-postmottagare för att avgöra om ett e-postmeddelande skickades av vem det skickades av. DKIM förbättrar ofta leveransen av e-postmeddelanden till inkorgen eftersom en mottagare kan vara säker på att meddelandet inte är en förfalskning.

**Hur fungerar DKIM?**

När du har konfigurerat den offentliga nyckeln i din DNS-post och aktiverat den sändande domänen i avsnittet Admin (A), aktiverar vi anpassad DKIM-signering för dina utgående meddelanden, som kommer att innehålla en krypterad digital signatur med varje e-postmeddelande som vi skickar till dig (B). Mottagarna kan dekryptera den digitala signaturen genom att leta upp den&quot;offentliga nyckeln&quot; i den sändande domänens DNS (C). Om nyckeln i e-postmeddelandet motsvarar nyckeln i din DNS-post, är det troligare att den mottagande e-postservern accepterar e-postmeddelandet som skickas för din räkning.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Hur ställer jag upp DKIM?**

Se [Konfigurera en anpassad DKIM-signatur](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Läs mer om SPF och hur det fungerar](http://www.open-spf.org/Introduction/){target="_blank"}
>* [Är min SPF korrekt konfigurerad?](https://www.kitterman.com/spf/validate.html){target="_blank"}
>* [Använde jag rätt syntax?](http://www.open-spf.org/SPF_Record_Syntax/){target="_blank"}

