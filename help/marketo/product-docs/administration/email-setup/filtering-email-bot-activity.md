---
description: Filtrering av e-postsatsaktivitet - Marketo Docs - produktdokumentation
title: Filtrerar e-postsatsaktivitet
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Filtrerar e-postsatsaktivitet {#filtering-email-bot-activity}

Ibland kan aktiviteten för e-postrobot felaktigt blåsa upp e-postöppningen och klicka på data. Så här löser du det.

>[!NOTE]
>
>Använda [IAB/ABC International Spiders and Bots List](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/)alla öppna-/klickaktiviteter med en IP- eller användaragent som matchar något i den listan identifieras som båda aktiviteter och loggas inte i Marketo.

1. Klicka **Administratör**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicka **E-post**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicka på **Rotaktivitet** -fliken.

   ![](assets/filtering-email-bot-activity-3.png)

1. Klicka på skjutreglaget för att aktivera **Filtrera startaktivitet**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Du kan välja separat om du vill att båda aktiviteterna ska loggas eller inte. Om du väljer att inte göra det kan du se en nedgång i e-postmeddelandet öppnas och klicka på falska siffror filtreras bort.

**VALFRITT STEG**: Om du vill inaktivera funktionen avmarkerar du bara reglaget. Om du avaktiverar funktionen &quot;Bot Activity in last 90 days&quot; utförs **not** återställ.

>[!TIP]
>
>Utnyttja data om robotaktivitet i smarta listor med booleska värdet&quot;Is Bot Activity&quot; (ja/nej), eller med tillämpliga filter-/utlösarbegränsningar.
