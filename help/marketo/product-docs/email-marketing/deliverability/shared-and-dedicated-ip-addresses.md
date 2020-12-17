---
unique-page-id: 10912085
description: Delade och dedikerade IP-adresser - Marketo Docs - Produktdokumentation
title: Delade och dedikerade IP-adresser
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Delade och dedikerade IP-adresser {#shared-and-dedicated-ip-addresses}

## Vad är en IP-adress? {#what-is-an-ip-address}

En numerisk etikett som anger adressen till en dator som är ansluten till Internet.

## Vad är delade IP-adresser? {#what-are-shared-ip-addresses}

Detta avser när flera avsändare använder samma IP-adresser för att starta e-postkampanjer. De delar alla samma sändande IP-adresser.

## Vad är en dedikerad IP-adress? {#what-is-a-dedicated-ip-address}

En användarspecifik IP-adress som bara en avsändare skickar från.

## Vilken är bäst - delad eller dedikerad? {#which-is-better-shared-or-dedicated}

Som vanligt finns det för- och nackdelar med båda alternativen.

**Pros and Cons of a Dedicated IP**

*Proffs*

**Anseende**  - Du äger ditt rykte och din leveransförmåga.\
**Övervakning**  - Med övervakning av leveransrapporter kan ni snabbt reagera på förändringar i leveransstatistiken.\
**Problemlösning**  - Det är enklare att undersöka, förstå och lösa leveransproblem.

*Kon*

**Volymförändringar**  - Volymtoppar kan påverka ditt rykte negativt och behöver hanteras.\
**IP-uppvärmningsprocess**  - Anseendet byggs över tid. En del internetleverantörer (ISP) stryper IP-adresser utan historik för volymer, så du måste skapa ett rykte under de första veckorna (Marketo kan hjälpa dig).\
**Kostnad**  - Det brukar tillkomma en extra kostnad att skicka från en dedikerad IP-adress till någon annan leverantör.

**Pros and Cons of a Shared IP**

*Proffs*

**Bra rumskompisar **- Om de personer du delar din IP-adress med följer vedertagna sändningsmetoder har du nytta av detta.\
**Utskicksfrekvens **- Det behövs ingen minsta utskicksfrekvens för att kvalificera sig för en delad IP, till skillnad från för dedikerade IP-adresser.\
**Kostnad **- Det tillkommer aldrig någon extra kostnad att skicka från en delad IP.

*Kon*

**Felaktiga rumskompisar**  - Om de personer du delar med dig av din IP-adress använder dåliga sändningsrutiner kan era e-postkampanjer påverkas negativt.\
**Kontroll **- Du har mycket mindre kontroll över avsändarens anseende.\
**Problemlösning **- Det kan ofta vara svårare att lösa ett problem när man skickar från delade IP-adresser.

>[!NOTE]
>
>När du fattar ett beslut finns det en annan viktig faktor att tänka på: sändande volym. Om du planerar att skicka mindre än 100 000 e-postmeddelanden per månad eller mindre än två utskick per månad, skulle du förmodligen inte ha någon dedikerad IP-adress. Att skicka siffror som detta anses lågt och det skulle vara svårt att hålla den dedikerade IP-adressen &quot;varm&quot; nog för att anses vara säker av de viktigaste internetleverantörerna. Om du inte skickar tillräckligt mycket post kommer internetleverantörerna att se ett utskick som en plötslig ökning av aktivitet och kan i slutänden blockera det som misstänkt spam.

Om du har några frågor, eller är intresserad av att konfigurera en dedikerad IP-adress, kontaktar du din Marketo-säljare.