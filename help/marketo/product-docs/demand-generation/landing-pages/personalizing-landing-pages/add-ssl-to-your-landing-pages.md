---
unique-page-id: 2359828
description: Lägg till SSL på era landningssidor - Marketo Docs - produktdokumentation
title: Lägg till SSL på era landningssidor
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: d5993d7c638994ea93446d20cbd1f1ae0b25e622
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Lägg till SSL på era landningssidor {#add-ssl-to-your-landing-pages}

Med SSL-kryptering (Secure Socket Layer) kan du skydda alla dina landningssidor för en Marketo Engage-instans.

När du fyller i ett webbformulär eller besöker en landningssida som hanteras av Marketo Engage, skickas informationen som standard via ett osäkert protokoll (HTTP). Enligt företagets policy kanske du vill skydda den information som skickas till Marketo via HTTPS. Om du till exempel besöker `http://info.mydomain.com/` det kommer nu att `https://info.mydomain.com/`.

Marketo Engage spårar&quot;Besökt webbsida&quot; och&quot;Klicka på länk på webbsida&quot; som standard över osäkra HTTP-protokoll. Om du vill att dina spårningslänkar ska vara skyddade med deras egna certifikat måste du ha Marketo som en separat icke-delad server för att kunna aktivera den. För att skydda alla aspekter av en kontakts interaktion med dig måste du vanligtvis skydda både landningssidor och spårningslänkar.

I slutet av 2022 ändrades hur landningssidans och spårningslänkens domäner skyddas. [Läs om dem här](https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305){target="_blank"}.

Om du vill ha SSL för dina landningssidor för Marketo Engage kontaktar du kontoteamet på Adobe (din kontoansvarige).
