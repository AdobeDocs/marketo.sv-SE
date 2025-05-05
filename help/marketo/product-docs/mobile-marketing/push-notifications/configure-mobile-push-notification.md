---
unique-page-id: 7512454
description: Konfigurera push-meddelanden för mobiler - Marketo Docs - produktdokumentation
title: Konfigurera push-meddelanden för mobilen
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 7007c9f61bac2d5b860e166f285c87f565683933
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Konfigurera push-meddelanden för mobilen {#configure-mobile-push-notification}

1. Gå till området **Marknadsföringsaktiviteter**.

   ![](assets/configure-mobile-push-notification-1.png)

1. Markera din push-resurs och klicka på **Redigera utkast**.

   ![](assets/configure-mobile-push-notification-2.png)

1. Välj önskat program i **Konfigurera**. Android- och Apple-plattformar är aktiverade som standard.

   ![](assets/configure-mobile-push-notification-3.png)

   >[!NOTE]
   >
   >Om ditt push-meddelande endast gäller för en plattform (t.ex. iOS) kan du utesluta den andra plattformen genom att manuellt skjuta dess väljare till **Inaktiverad**.

1. Klicka på **Nästa**.

   ![](assets/configure-mobile-push-notification-4.png)

1. Ange meddelandetext eller välj tokeikonen för att lägga till tokens (i den här redigeraren formateras [ eftersom de vanligtvis är ](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) - du kan använda flera token). Välj en **Tryck på åtgärd**.

   ![](assets/configure-mobile-push-notification-5.png)

   >[!NOTE]
   >
   >Om en plattform är aktiverad visas den till vänster på telefonskärmen. Den visas i färg när den är markerad.

   >[!NOTE]
   >
   >Det finns tre typer av Tap-åtgärder:
   >
   >**Starta appen** - **Den här appen** öppnar appens startsida när användaren trycker på meddelandet. **Anpassad** använder en djuplänk för att öppna andra områden i din app eller något annat program som du har länken till (mer information finns i [Deep Link URI:er](#deep-link-uris) nedan).
   >
   >**Landningssida** - tar dig till en angiven Marketo-landningssida.
   >
   >**Extern URL** - tar dig till en landningssida som inte är Marketo.

1. Om du vill infoga en djuplänk för en anpassad knackningsåtgärd väljer du **Anpassad** och anger [djuplänkens URI](#deep-link-uris) i fältet.

   ![](assets/configure-mobile-push-notification-6.png)

   >[!NOTE]
   >
   >Meddelanden och Tryck på Åtgärder ser likadana ut på båda plattformarna.

1. Endast för iOS markerar du kryssrutan för att ange att programmet ska spela upp ett ljud när meddelandet kommer. Android spelar upp ljudet automatiskt.

   ![](assets/configure-mobile-push-notification-7.png)

1. Förhandsgranska den andra plattformen och klicka på **Slutför**.

   ![](assets/configure-mobile-push-notification-8.png)

1. Klicka på **Godkänn och stäng**.

   ![](assets/configure-mobile-push-notification-9.png)

Grattis! Nu är push-meddelandet klart att skickas.

## Deep Link URIs {#deep-link-uris}

När prenumeranter klickar på en knapp i ett push-meddelande kan de antingen gå till appens hemsida eller direkt till en viss sida i appen. En djup länk är en unik referens till en viss sida i appen och ser ut ungefär som en webbplatslänk.

En URI med djup länk består av tre delar: schemanamn, sökväg och identifierare. I exemplet nedan är &quot;myappname&quot; schemat. &quot;products&quot; is the path, and &quot;purple-shirts&quot; is the identifier. När kunden knackar tas de specifikt till den lila skjortan på appens produktsidor.

![](assets/configure-mobile-push-notification-10.png)

Programmets djuplänksstruktur kan dock skilja sig från ovanstående exempel. Din utvecklare har många alternativ för att definiera URI:er för djuplänk, så be utvecklaren att skicka URI:er (länkar) till de sidor som du är intresserad av att använda. Detta garanterar att de URI:er som du anger i push-meddelanden pekar på rätt platser. Din utvecklare kan [hitta mer information här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Skicka ett mobilpush-meddelande](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
