---
unique-page-id: 14352477
description: Skicka till  [!DNL Sales Connect] - Marketo Docs - produktdokumentation
title: Skjut till  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 2%

---

# Skjut till [!DNL Sales Connect] {#push-to-sales-connect}

Knappen [!UICONTROL Push to Tout] tar en lista över dina leads/kontakter i [!DNL Salesforce] och överför dem till en grupp i [!DNL Sales Connect]. Du kan sedan snabbt skicka en anpassningsbar gruppe-post med Tout-spårning bifogad.

## Krav {#requirements}

* [!DNL Sales Connect Salesforce]-paket som installerats av [!DNL Salesforce] Admin

* [!UICONTROL Push to Sales Connect]-knappen har installerats i listvyn av [!DNL Salesforce] Admin

* [!DNL Salesforce]-anslutning skapad med [!DNL Sales Connect] för användare som gör penseln

## Använda {#how-to}

1. Klicka på fliken **[!UICONTROL Lead/Contact]** i [!DNL Salesforce].
1. Växla till listvyn som du vill skicka till [!DNL Sales Connect] bredvid knappen [!UICONTROL Go].
1. Klicka på **[!UICONTROL Go]**.
1. Markera alla leads/kontakter som du vill ska pushas för tout.
1. Välj **[!UICONTROL Push to MSE]**.
1. Ett nytt fönster visas som verifierar antalet leads/kontakter som du vill skicka över. Välj **[!UICONTROL Proceed to Group]**.[!DNL Sales Connect] kommer inte att föra över kontakter som är markerade som [!UICONTROL Email Opt Out] i [!DNL Salesforce] eller [!UICONTROL Unsubscribed] i [!DNL Sales Connect].

   >[!NOTE]
   >
   >[!DNL Sales Connect] lägger till den här gruppen med namnet&quot;SFDC-..&quot; på sidan Relationer i [webbprogrammet](https://toutapp.com/login).

1. Välj **[!UICONTROL Email Entire Group]** om du vill skicka ut gruppe-postmeddelandet.
