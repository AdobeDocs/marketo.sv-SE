---
solution: Marketo Engage
product: marketo
title: Personalization Tokens
description: Läs om hur du använder personaliseringstoken i nya Marketo Engage Email Designer
level: Beginner, Intermediate
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
source-git-commit: 5575ab0d7141d4bfc610430db625439c9f52e231
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Personalization Tokens {#personalization-tokens}

E-postdesignern har ett annat format än den klassiska e-postredigeraren när det gäller token för e-postanpassning. Ändringen implementerades för att förbättra kompatibiliteten med Handlebar-skript och effektivisera skapandet av e-postmeddelanden.

>[!AVAILABILITY]
>
>Från och med 23 maj 2025 kommer den här funktionen att distribueras till Marketo Engage-användare i grupper, med en region uppdaterad per vecka. Under utrullningen kommer e-postmeddelanden som skapas med den nya e-postdesignern automatiskt att migrera befintliga tokens till det nya formatet. Med den här uppdateringen kommer alla tokens endast att vara tillgängliga på engelska.

## Primär användning {#primary-use-case}

Den här förbättringen är främst till nytta för övergången från [hastighetsskript](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/email-scripting){target="_blank"} till Handlebar-skript. Den nya e-postdesignern har bara stöd för det nya tokenformatet. Det uppdaterade formatet eliminerar blanksteg och lägger till en reviderad standardtextstruktur, vilket ger en smidigare och effektivare skriptupplevelse.

## Tokenupplevelse {#token-experience}

En titt på tokenupplevelsen, både gammal och ny.

### Gammalt format {#old-format}

I den klassiska e-postredigeraren kan du lägga till variabler med mellanslag, till exempel `lead.Anonymous IP` eller `member.registration code`. Standardtextens format var: `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### Nytt format {#new-format}

I e-postdesignern måste du använda [kamelcase](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) eller understreck för tokens (t.ex. `lead.anonymousIP` eller `member.registration_code`). Formatet för standardtexten ändras också till `{%=lead.city ?: "fallback" %}`.

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## Saker att notera {#things-to-note}

* Anpassningsredigeraren har även följande funktioner som underlättar redigeringen:

   * Ångra/gör om
   * Sök/Sök och ersätt
   * Komplettera automatiskt

* **Alla**-token som tidigare hade stöd i Marketo Engage stöds i den nya personaliseringsredigeraren.
