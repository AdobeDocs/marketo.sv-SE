---
unique-page-id: 11376159
description: Innan du skapar push-meddelanden och meddelanden i appen - Marketo Docs - produktdokumentation
title: Innan du skapar push-meddelanden och meddelanden i appen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# Innan du skapar push-meddelanden och meddelanden i appen {#before-you-create-push-notifications-and-in-app-messages}

Det är inte svårt att skapa push-meddelanden och meddelanden i appen, men du måste ha allt klart innan du kan börja. Marketo Admin och utvecklare av mobilappar ska följa stegen nedan för att förbereda nödvändiga integreringar.

1. Först lägger Marketo Admin [till en mobilapp](add-a-mobile-app.md)
1. Marketo Admin skickar sedan [ett kodfragment till utvecklaren](send-sdk-code-to-a-developer.md)
1. Utvecklaren hämtar SDK-filen och inkluderar fragment och andra metoder för [Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) eller [iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. Som standard utlöses meddelanden i appen när appen öppnas. Om du vill utlösa meddelanden för andra händelser, till exempel när en viss sida visas eller en viss knapp skickas, måste utvecklaren lägga till anpassade händelser i koden (se [Anpassade händelser för meddelanden i appen](#CustomEvents) nedan)
1. Utvecklaren [genererar nyckel och projektnummer för server-API för Android](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) eller [certifiering och lösenord för iOS](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) och skickar den till Marketo Admin
1. Marketo Admin konfigurerar push-meddelandeåtkomst [med Server-API-nyckeln (Android)](configure-mobile-app-android-push-access.md) eller [med certifikatet (iOS)](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>Det är enkelt för Marketo Admin att kontrollera om din push-konfiguration har verifierats. Gå [hit](verify-push-configuration.md).

## Anpassade händelser för meddelanden i appen {#custom-events-for-in-app-messages}

För meddelanden i programmet är visningsutlösaren inställd på **App Open** som standard. Om du vill använda anpassade händelser för att utlösa visningen av meddelanden i appen (till exempel **Klicka på Lägg till i kundvagnen**, **sidan Vyinställningar**) skapar du en lista över önskade händelser och ger den till din mobilappsutvecklare. Utvecklaren lägger sedan till anpassade händelser i koden. När de har godkänts visas de som visningsutlösare när du ställer in målgruppen. **Varning**: Godkännandeprocessen för anpassad händelsekodning kan ta lite tid att slutföra.

När du har gjort alla förberedelser för meddelanden i appen och push-meddelanden är det dags att komma igång!

>[!MORELIKETHIS]
>
>* [Skapa ett meddelande i appen](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Skapa ett push-meddelande](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



