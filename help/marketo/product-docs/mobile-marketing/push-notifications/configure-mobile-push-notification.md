---
description: Konfigurera push-meddelanden för mobiler - Marketo Docs - produktdokumentation
title: Konfigurera push-meddelanden för mobilen
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: f6bdae9dbf1520bd8f30b4dd774b52a36b029c45
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Konfigurera push-meddelanden för mobilen {#configure-mobile-push-notification}

1. Gå till området **[!UICONTROL Marketing Activities]**.

   ![](assets/configure-mobile-push-notification-1.png)

1. Välj din push-resurs och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/configure-mobile-push-notification-2.png)

1. Välj önskat program i **Konfigurera**. Android- och Apple-plattformar är aktiverade som standard.

   ![](assets/configure-mobile-push-notification-3.png)

   >[!NOTE]
   >
   >Om ditt push-meddelande endast gäller för en plattform (till exempel iOS) kan du utesluta den andra plattformen genom att manuellt skjuta dess väljare till **Inaktiverad**.

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/configure-mobile-push-notification-4.png)

1. Ange meddelandetext eller välj tokeikonen för att lägga till tokens (i den här redigeraren formateras [&#x200B; eftersom de vanligtvis är &#x200B;](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) - du kan använda flera token). Välj en **Tryck på åtgärd**.

   ![](assets/configure-mobile-push-notification-5.png)

   >[!NOTE]
   >
   >Om en plattform är aktiverad visas den till vänster på telefonskärmen. Den visas i färg när den är markerad.

   >[!NOTE]
   >
   >Det finns tre typer av [!UICONTROL Tap Actions]:
   >
   >**Starta appen** - **Den här appen** öppnar appens startsida när användaren trycker på meddelandet. **Anpassad** använder en djuplänk för att öppna andra områden i din app eller något annat program som du har länken till (mer information finns i [Deep Link URI:er](#deep-link-uris) nedan).
   >
   >**[!UICONTROL Landing Page]** - tar dig till en angiven Marketo-landningssida.
   >
   >**[!UICONTROL External URL]** - tar dig till en landningssida som inte är Marketo.

1. Om du vill infoga en djuplänk för en anpassad knackningsåtgärd väljer du **Anpassad** och anger [djuplänkens URI](#deep-link-uris) i fältet.

   ![](assets/configure-mobile-push-notification-6.png)

1. För iOS markerar du kryssrutan för att ange att programmet ska spela upp ett ljud när meddelandet kommer. Android spelar upp ljudet automatiskt.

   ![](assets/configure-mobile-push-notification-7.png)

1. Förhandsgranska den andra plattformen och klicka på **[!UICONTROL Finish]**.

   ![](assets/configure-mobile-push-notification-8.png)

1. Klicka på **[!UICONTROL Approve and Close]**.

   ![](assets/configure-mobile-push-notification-9.png)

Push-meddelandet är klart att skickas.

Om du får felmeddelandet `Limited Access: You do not have sufficient privileges to perform this action` kontrollerar du att behörigheten **Access Design Studio** > `Access Landing Page` har angetts för användaren, plus minst ett av följande:

* Godkänn push-meddelande
* Ta bort push-meddelande
* Redigera push-meddelande

## Deep Link URIs {#deep-link-uris}

När prenumeranter klickar på en knapp i ett push-meddelande kan de antingen gå till appens hemsida eller direkt till en viss sida i appen. En djup länk är en unik referens till en viss sida i appen och ser ut ungefär som en webbplatslänk.

En URI med djup länk består av tre delar: schemanamn, sökväg och identifierare. I exemplet nedan är &quot;myappname&quot; schemat. &quot;products&quot; is the path, and &quot;purple-shirts&quot; is the identifier. När kunden knackar tas de specifikt till den lila skjortan på appens produktsidor.

![](assets/configure-mobile-push-notification-10.png)

Programmets djuplänksstruktur kan dock skilja sig från ovanstående exempel. Din utvecklare har många alternativ för att definiera djuplänks-URI:er, så be din utvecklare att skicka URI:er (länkar) till de sidor som du är intresserad av att använda. Detta garanterar att de URI:er som du anger i push-meddelanden pekar på rätt plats. Din utvecklare kan [hitta mer information här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Skicka ett mobilpush-meddelande](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
