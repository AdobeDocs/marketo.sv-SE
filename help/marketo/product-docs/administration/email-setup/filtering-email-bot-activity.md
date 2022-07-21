---
description: Filtrering av e-postsatsaktivitet - Marketo Docs - produktdokumentation
title: Filtrerar e-postsatsaktivitet
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 524e185e255503ac44bb73303091a59b2d60242a
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Filtrerar e-postsatsaktivitet {#filtering-email-bot-activity}

Ibland kan aktiviteten för e-postrobot felaktigt blåsa upp e-postöppningen och klicka på data. Åtgärda problemet genom att följa stegen nedan.

Vi använder tre olika metoder för att bekräfta båda aktiviteterna:

* Matcha med [Interactive Advertising Bureau bot list](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;}: Aktiviteter som matchar något i listan IAB UA/IP (User Agent/IP address) markeras som bots.
* Matcha med närhetsmönster: När fler än två aktiviteter inträffar samtidigt (under två sekunder) identifieras de som bottar.

I e-postlänkens klickning och öppningsaktivitet via e-post fylls nya attribut med värdena nedan:

* Aktiviteter som identifieras som bottar har &quot;Bot Activity&quot; som &quot;True&quot; och &quot;Bot Activity Pattern&quot; som det identifierade mönstret/metoden
* Aktiviteter som inte identifieras som&quot;bottenaktivitet&quot; kommer att ha&quot;bottenaktivitet&quot; som&quot;falsk&quot; och&quot;bitaktivitetsmönster&quot; som&quot;inget/inget&quot;
* Aktiviteter som inträffade innan de här attributen introducerades har &quot;Rotaktivitet&quot; som &quot; (tom) och &quot;Punktaktivitetsmönster&quot; som &quot; (tom)

1. Klicka **Administratör**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicka **E-post**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicka på **Rotaktivitet** -fliken.

   ![](assets/filtering-email-bot-activity-3.png)

1. Välj **Matcha med IAB-lista**, **Matcha med närhetsmönster** eller båda.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Du kan välja att filtrera båda aktiviteterna **eller** loggad. Om du väljer filtrerad kan du se en nedgång i e-postmeddelanden som öppnas och klicka på falska aktiviteter som försvinner

**VALFRITT STEG**: Om du vill inaktivera den här funktionen avmarkerar du reglagen. Om du inaktiverar återställs inte data.

>[!TIP]
>
>Utnyttja informationen om robotaktivitet i smarta listor via boolesk aktivitet (ja/nej) och Bot Activity Pattern (Bot Activity Pattern) i filtren&quot;Click Link in Email&quot; och&quot;Open Email&quot; (Öppna e-post) och&quot;Click Link in Email&quot; och&quot;Open Email&quot; (Öppna e-post).
