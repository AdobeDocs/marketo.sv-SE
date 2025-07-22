---
unique-page-id: 10099077
description: Lär dig hur du importerar en startvärdeslista till din Marketo Engage-instans.
title: Power Pack för e-postleverans - Så här importerar du en dirigeringslista
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Power Pack för e-postleverans: Så här importerar du en dirigeringslista {#email-deliverability-power-pack-how-to-import-a-seed-list}

En lista med dirigerade e-postkonton är en lista över e-postkonton hos flera postlådeproviders, inklusive Google Apps, Hotmail, Yahoo!, osv., som används för att beräkna hur många inkorgar och skräppostmappar som levereras. Här nedan beskrivs de steg som krävs för att få in den listan i din Marketo Engage-instans.

>[!IMPORTANT]
>
>Den här artikeln är avsedd för användare med en aktiv Everest-prenumeration just nu. Om du använder Inbox Tracker från Bird (tidigare MessageBird) hittar du dina självstudiekurser [här](/help/marketo/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.md){target="_blank"}.

## Importera en dirigerad lista {#import-a-seed-list}

1. Välj **[!UICONTROL Deliverability Tools]** i My Marketo.

   ![](assets/email-deliverability-power-pack-1.png)

1. Programmet [!DNL Everest] öppnas. Klicka på **[!UICONTROL In-Flight]** i den vänstra navigeringen och välj **[!UICONTROL Inbox Placement]**.

   ![](assets/email-deliverability-power-pack-2.png)

1. Klicka på fliken **[!UICONTROL Manage Seed List]**.

   ![](assets/email-deliverability-power-pack-3.png)

1. Klicka på listrutan **[!UICONTROL Actions]** och välj **[!UICONTROL Download: One Per Line]**.

   ![](assets/email-deliverability-power-pack-4.png)

   >[!NOTE]
   >
   >Använd optimeringsfunktionen för dirigerad lista (längst upp på sidan) om du vill att [!DNL Everest] ska optimera listan åt dig.

1. Efter exporten visas listan som en TXT-fil i webbläsarens nedladdningsmapp. Hämta den och [importera](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) den till din Marketo-instans som en statisk lista.

   ![](assets/email-deliverability-power-pack-5.png)

   >[!TIP]
   >
   >Ge listan ett namn som gör det enkelt att hitta.

   >[!CAUTION]
   >
   >Du får ett begränsat antal av dessa kampanjer för inkorgsplacering per månad. Titta på avsnittet [!UICONTROL Subscription] under [!UICONTROL Account Settings] > [!UICONTROL Subscription] i [!DNL Everest] om du vill se hur många du får. Kontakta din Marketo-säljare om du vill ha mer information.

## Hämtar nya dirigeringslistor {#acquiring-new-seedlists}

Din dirigeringslista kan ändras så ofta som varje månad. Det är viktigt att du regelbundet loggar in på e-postleverantörens Power Pack och kontrollerar statusen för din dirigeringslista. När nya adresser läggs till eller en uppdatering krävs får du ett meddelande via meddelandeikonen längst ned till vänster i programmet.

När den statiska listan i Marketo har skapats kan du börja skicka till den för att testa e-postens placering i inkorgen.
