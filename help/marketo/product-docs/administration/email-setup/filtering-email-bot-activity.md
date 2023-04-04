---
description: Filtrering av e-postsatsaktivitet - Marketo Docs - produktdokumentation
title: Filtrerar e-postsatsaktivitet
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 792db38ec0891d4a6de5a8d0bd746bd7bb429edb
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 3%

---

# Filtrerar e-postsatsaktivitet {#filtering-email-bot-activity}

Ibland kan aktiviteten för e-postrobot felaktigt blåsa upp e-postöppningen och klicka på data. Åtgärda problemet genom att följa stegen nedan.

Vi använder tre olika metoder för att bekräfta båda aktiviteterna:

* Matcha med [Interactive Advertising Bureau bot list](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: Aktiviteter som matchar något i listan IAB UA/IP (User Agent/IP address) markeras som bots.
* Matcha med närhetsmönster: När fler än två aktiviteter inträffar samtidigt (på mindre än en sekund) identifieras de som bottar. Attribut som beaktas vid jämförelse är:
   * Lead-ID (ska vara samma)
   * E-postresurs (ska vara samma)
   * Klicka eller mejla
   * Tidsskillnad (bör vara mindre än en sekund)

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

1. Välj **Matcha med IAB-lista**, **Matcha med närhetsmönster** eller båda. Välj om startaktivitet ska loggas _eller_ filterrobotaktivitet.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Om du väljer Filtrera startaktivitet kan du se en nedgång i e-postmeddelandet som öppnas och klicka på som falska aktiviteter uteslöts.

**VALFRITT STEG**: Om du vill inaktivera den här funktionen avmarkerar du reglagen. Om du inaktiverar återställs inte data.

>[!TIP]
>
>Utnyttja informationen om robotaktivitet i smarta listor via boolesk aktivitet (ja/nej) och Bot Activity Pattern (Bot Activity Pattern) i filtren&quot;Click Link in Email&quot; och&quot;Open Email&quot; (Öppna e-post) och&quot;Click Link in Email&quot; och&quot;Open Email&quot; (Öppna e-post).

## IP Blockeringslista {#ip-blocklist}

Vi har sammanställt en lista med IP-adresser som ansvarar för att generera miljontals falska åtaganden, eftersom ett sådant engagemang som tas emot från någon av följande IP-adresser automatiskt filtreras bort och inte läggs till i din Marketo Engage-instans. Detta kan leda till att e-postöppningar, klick och andra relaterade aktiviteter minskar. Listan nedan kan uppdateras regelbundet.

* 209.222.82.126
* 209.222.82.127
* 209.222.82.128
* 209.222.82.129
* 209.222.82.138
* 209.222.82.139
* 209.222.82.140
* 209.222.82.141
* 209.222.82.228
* 209.222.82.229
* 209.222.82.230
* 209.222.82.231
* 209.222.82.232
* 209.222.82.233
* 209.222.82.234
* 209.222.82.235

>[!NOTE]
>
>Vi analyserar och undersöker noggrant varje IP-adress innan vi lägger till den i listan, så att bara de mest kritiska och skadliga IP-adresserna blockeras.
