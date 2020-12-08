---
unique-page-id: 7512454
description: Konfigurera Mobile Push Notification - Marketo Docs - produktdokumentation
title: Konfigurera push-meddelanden för mobilen
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Konfigurera push-meddelanden för mobilen {#configure-mobile-push-notification}

1. Gå till området Marknadsföringsaktiviteter.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Markera din push-resurs och klicka på **Redigera utkast**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Gå till **Konfigurera**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Välj önskat program. Android- och Apple-plattformarna är aktiverade som standard.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

   Om ditt push-meddelande endast gäller för en plattform (till exempel för iPhone) kan du utesluta den andra plattformen genom att skjuta dess väljare till Inaktiverad.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

   Klicka på NÄSTA.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Ange meddelandetext eller välj token-ikonen om du vill lägga till variabler. Välj sedan en **knackåtgärd**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Om en plattform är aktiverad visas den till vänster på telefonskärmen. Den visas i färg när den är markerad.

   >[!NOTE]
   >
   >**Definition**
   >
   >
   >Det finns tre typer av** Tryck på Åtgärder:**
   >
   >
   >**Starta app** - **Den här appen** öppnar appens startsida när användaren trycker på meddelandet. **Anpassad** använder en djuplänk för att öppna andra områden i din app eller andra appar som du har länken till (mer information finns i [Deep Link URI](#Deeplink) nedan).
   >
   >
   >**Landningssida** - tar dig till en angiven Marketo-landningssida.
   >
   >
   >**Extern URL** - tar dig till en landningssida som inte är markerad.

   Om du vill infoga en djuplänk för en anpassad knackningsåtgärd klickar du på Anpassad och anger [djuplänkens URI](#Deeplink) i fältet.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

   Om du vill infoga variabler väljer du en token, anger ett standardvärde och klickar på Infoga.

   >[!NOTE]
   >
   >Token visas där du placerar markören i textrutan. Du kan använda mer än en token.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Meddelanden och Tryck på Åtgärder ser likadana ut på båda plattformarna.

   För iOS markerar du kryssrutan för att ange att programmet ska spela upp ett ljud när meddelandet kommer. Android spelar upp ljudet automatiskt.

   ![](assets/ios-tap-and-notification-hand.png)

   Förhandsgranska den andra plattformen och klicka på FINISH.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Klicka på **GODKÄNN OCH STÄNG**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Grattis! Nu är push-meddelandet klart att skickas.

## Deep Link URIs {#deep-link-uris}

När prenumeranter klickar på en knapp i ett push-meddelande kan de antingen gå till appens hemsida eller direkt till en viss sida i appen. En djup länk är en unik referens till en viss sida i appen och ser ut ungefär som en webbplatslänk.

En djuplänk-URI består av tre delar: schemanamn, sökväg och identifierare. I exemplet nedan är &quot;myappname&quot; schemat. &quot;products&quot; is the path, and &quot;purple-shirts&quot; is the identifier. När kunden knackar tas de specifikt till den lila skjortan på appens produktsidor.

![](assets/image2016-7-29-12-3a49-3a1.png)

Programmets djuplänksstruktur kan dock skilja sig från ovanstående exempel. Din utvecklare har många alternativ för att definiera URI:er för djuplänk, så be utvecklaren att skicka URI:er (länkar) till de sidor som du är intresserad av att använda. Detta garanterar att de URI:er som du anger i push-meddelanden pekar på rätt platser. Din utvecklare kan [hitta mer information här](http://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Skicka ett mobilpush-meddelande](send-a-mobile-push-notification.md)

>



