---
unique-page-id: 11376159
description: Innan du skapar push-meddelanden och meddelanden i appen - Marketo Docs - produktdokumentation
title: Innan du skapar push-meddelanden och meddelanden i appen
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Innan du skapar push-meddelanden och meddelanden i appen {#before-you-create-push-notifications-and-in-app-messages}

Det är inte svårt att skapa push-meddelanden och meddelanden i appen, men du måste ha allt klart innan du kan börja. Marketo Admin och utvecklaren av mobilappar följer stegen nedan för att förbereda nödvändiga integreringar.

1. Först lägger Marketo Admin [till en mobilapp](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Marketo Admin [skickar sedan ett kodfragment till utvecklaren](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Utvecklaren hämtar SDK och inkluderar kodfragment och andra metoder för [Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) eller [iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios).

1. Som standard utlöses meddelanden i appen när appen öppnas. Om du vill utlösa meddelanden för andra händelser, till exempel när en viss sida visas eller en viss knapp skickas, måste utvecklaren lägga till anpassade händelser i koden (se [Anpassade händelser för meddelanden i appen](#CustomEvents) nedan).

1. Utvecklaren [genererar nyckel och projektnummer för server-API för Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) eller [ för certifiering och lösenord för iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) och skickar den till Marketo Admin.

1. Marketo Admin konfigurerar push-meddelandeåtkomst [med Server-API-nyckeln (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) eller [ med certifikatet (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Det är enkelt för en Marketo-administratör att kontrollera om din push-konfiguration har verifierats. Gå [hit](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md) bara.

## Anpassade händelser för meddelanden i appen {#custom-events-for-in-app-messages}

För meddelanden i programmet är visningsutlösaren inställd på **[!UICONTROL App Open]** som standard. Om du vill använda anpassade händelser för att utlösa visningen av meddelanden i appen (till exempel **Klicka på Lägg till i kundvagnen**, **sidan Vyinställningar**) skapar du en lista över önskade händelser och ger den till din mobilappsutvecklare. Utvecklaren lägger sedan till anpassade händelser i koden. När de har godkänts visas de som visningsutlösare när du ställer in målgruppen. **Varning**: Det kan ta ett tag att slutföra den anpassade händelsekodningsprocessen.

När du har gjort alla förberedelser för meddelanden i appen och push-meddelanden är det dags att komma igång!

>[!MORELIKETHIS]
>
>* [Skapa ett meddelande i appen](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Skapa ett push-meddelande](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
