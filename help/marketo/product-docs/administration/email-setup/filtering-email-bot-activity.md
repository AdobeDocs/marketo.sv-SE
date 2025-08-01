---
description: Filtrering av e-postsatsaktivitet - Marketo Docs - produktdokumentation
title: Filtrerar e-postsatsaktivitet
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
feature: Email Setup
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Filtrerar e-postsatsaktivitet {#filtering-email-bot-activity}

Ibland kan aktiviteten för e-postrobot felaktigt blåsa upp e-postöppningen och klicka på data. Åtgärda problemet genom att följa stegen nedan.

Vi använder två olika metoder för att bekräfta båda aktiviteterna:

* Matcha med [Interactive Advertising Bureau bot list](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: Aktiviteter som matchar något i IAB UA/IP-listan (User Agent/IP address) markeras som bots.
* Matcha med närhetsmönster: När två eller flera aktiviteter inträffar samtidigt (under en sekund) identifieras de som botar. Attribut som beaktas vid jämförelse är:
   * Lead-ID (ska vara samma)
   * E-postresurs (ska vara samma)
   * Klicka eller mejla
   * Tidsskillnad (bör vara mindre än en sekund)

I e-postlänkens klickning och öppningsaktivitet via e-post fylls nya attribut med värdena nedan:

* Aktiviteter som identifieras som bottar har &quot;Bot Activity&quot; som &quot;True&quot; och &quot;Bot Activity Pattern&quot; som det identifierade mönstret/metoden
* Aktiviteter som inte identifieras som&quot;bottenaktivitet&quot; kommer att ha&quot;bottenaktivitet&quot; som&quot;falsk&quot; och&quot;bitaktivitetsmönster&quot; som&quot;inget/inget&quot;
* Aktiviteter som inträffade innan de här attributen introducerades har &quot;Rotaktivitet&quot; som &quot; (tom) och &quot;Punktaktivitetsmönster&quot; som &quot; (tom)

## Välj filtertyp {#select-filter-type}

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicka på fliken **[!UICONTROL Bot Activity]**.

   ![](assets/filtering-email-bot-activity-3.png)

1. Det finns två reglage att välja mellan. Du kan bara aktivera en eller båda. Om du aktiverar **[!UICONTROL Match with IAB List]** väljer du om du vill [!UICONTROL log bot activity] _eller_ [!UICONTROL filter bot activity].

   ![](assets/filtering-email-bot-activity-4.png)

1. Om du aktiverar **[!UICONTROL Match with Proximity Pattern]** väljer du om du vill [!UICONTROL log bot activity] _eller_ [!UICONTROL filter bot activity]. Du kan också ange antalet sekunder för **Varaktighet mellan aktiviteter** (standard är 0, max är 3).

   ![](assets/filtering-email-bot-activity-5.png)

>[!NOTE]
>
>Med **Varaktighet mellan aktiviteter** inställd på 0 sekunder kommer vi att identifiera e-postaktiviteter som inträffar exakt samma sekund. Om flera e-postaktiviteter inträffar inom det angivna antalet sekunder identifieras de som en Båda-aktivitet.

>[!IMPORTANT]
>
>* Om du väljer [!UICONTROL Filter Bot Activity] kan du se en nedgång i e-postmeddelanden som öppnas och klicka på falska aktiviteter som försvinner.

**VALFRITT STEG**: Om du vill inaktivera någon av funktionerna avmarkerar du bara respektive skjutreglage. Om du gör det återställs inte data.

>[!TIP]
>
>Utnyttja informationen om robotaktivitet i smarta listor via boolesk aktivitet (ja/nej) och Bot Activity Pattern (Bot Activity Pattern) i filtren&quot;Click Link in Email&quot; och&quot;Open Email&quot; (Öppna e-post) och&quot;Click Link in Email&quot; och&quot;Open Email&quot; (Öppna e-post).

## IP BLOCKERINGSLISTA {#ip-blocklist}

Vi har sammanställt en lista med IP-adresser som ansvarar för att generera miljontals falska åtaganden, eftersom ett sådant engagemang som tas emot från någon av följande IP-adresser automatiskt filtreras bort och inte läggs till i din Marketo Engage-instans. Detta kan leda till att e-postöppningar, klick och andra relaterade aktiviteter minskar. Listan nedan kan uppdateras regelbundet.

* 40.94.34.52
* 40.94.34.86
* 52.34.76.65
* 54.70.53.60
* 54.71.187.124
* 60.28.2.248
* 64.235.150.252
* 64.235.153.10
* 64.235.153.2
* 64.235.154.105
* 64.235.154.109
* 64.235.154.140
* 64.74.215.1
* 64.74.215.100
* 64.74.215.138
* 64.74.215.139
* 64.74.215.142
* 64.74.215.146
* 64.74.215.150
* 64.74.215.154
* 64.74.215.158
* 64.74.215.162
* 64.74.215.164
* 64.74.215.166
* 64.74.215.170
* 64.74.215.174
* 64.74.215.176
* 64.74.215.178
* 64.74.215.51
* 64.74.215.56
* 64.74.215.58
* 64.74.215.59
* 64.74.215.86
* 64.74.215.98
* 65.154.226.101
* 66.249.91.149
* 70.42.131.106
* 74.125.217.116
* 74.217.90.250
* 104.129.41.4
* 104.47.55.126
* 104.47.58.126
* 104.47.70.126
* 104.47.73.126
* 104.47.73.254
* 104.47.74.126
* 128.220.160.1
* 155.70.39.101
* 162.129.251.14
* 162.129.251.42
* 208.52.157.204

>[!NOTE]
>
>Vi analyserar och undersöker noggrant varje IP-adress innan vi lägger till den i listan, så att bara de mest kritiska och skadliga IP-adresserna blockeras.
