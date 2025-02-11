---
unique-page-id: 11379622
description: Ställ in Facebook-annonser - Marketo Docs - produktdokumentation
title: Konfigurera Facebook-annonser
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 5b31abc52e9bba690e908d9ee6018cecad0080e7
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Konfigurera Facebook-annonser {#set-up-facebook-lead-ads}

Använd [Facebook Lead Ads](https://www.facebook.com/business/ads/ad-objectives/lead-generation){target="_blank"} för att köra annonskampanjer på Facebook och generera leads för Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!AVAILABILITY]
>
>Om du vill lägga till Facebook-annonser i din instans kontaktar du Adobe Account Team (din kontohanterare).

1. Gå till området **Admin** i Marketo Engage.

   ![](assets/set-up-facebook-lead-ads-1.png)

1. Gå till **LaunchPoint**, klicka på listrutan **Nytt** och välj **Ny tjänst**.

   ![](assets/set-up-facebook-lead-ads-2.png)

1. Ange ett **visningsnamn** för tjänsten, välj tjänsten **Facebook Lead Ads** i listrutan och klicka på **Create**.

   ![](assets/set-up-facebook-lead-ads-3.png)

1. Öppna en ny flik i samma webbläsare och gå till [facebook.com](https://www.facebook.com){target="_blank"}. Logga in på Facebook med det konto du vill använda för integreringen.

   >[!NOTE]
   >
   >Facebook-kontot måste ha tillgång till alla Facebook-affärssidor som du vill hämta leads från.

   ![](assets/set-up-facebook-lead-ads-4.png)

1. När du har loggat in på Facebook går du tillbaka till Marketo och klickar på **Auktorisera**.

   ![](assets/set-up-facebook-lead-ads-5.png)

1. Om du uppmanas till det klickar du på **OK** för att godkänna Marketo-appinstallationen till Facebook.

   ![](assets/set-up-facebook-lead-ads-6.png)

1. Du kommer att märka att du nu är auktoriserad. Klicka på **Nästa**.

   ![](assets/set-up-facebook-lead-ads-7.png)

1. Markera de sidor du vill att Marketo ska hämta Facebook-annonser från och klicka på **Nästa**.

   >[!TIP]
   >
   >Om du inte ser någon sida som du väntar dig ska du kontrollera att det Facebook-konto som används för att autentisera läggs till på sidan på Facebook och försöka igen.

   ![](assets/set-up-facebook-lead-ads-8.png)

1. Om du vill acceptera standardfältmappningar från Facebook till Marketo klickar du bara på **Skapa**.

   >[!TIP]
   >
   >Genom att ändra mappningarna kan du anpassa var informationen om annonser för leads lagras i Marketo. Du kan även [hämta in data från anpassade frågor för Lead Ads ](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md){target="_blank"}.

   >[!CAUTION]
   >
   >Marketo stöder inte mappning av två Facebook-fält till ett enda Marketo-fält, bara 1 till 1. Om du mappar 2 till 1 kan leads misslyckas med att ansluta till Marketo.

   ![](assets/set-up-facebook-lead-ads-9.png)

   Snyggt gjort! Leads kommer att börja flöda in i Marketo när ni genomför framgångsrika Facebook-annonskampanjer.

   ![](assets/set-up-facebook-lead-ads-10.png)

>[!MORELIKETHIS]
>
>* [Tilldela/ta bort behörigheter i hanteraren för leads (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862){target="_blank"}
>* [Använd filter och utlösare för annonsering på leads i en smart kampanj](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
>* [Mappa anpassade fält till Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md){target="_blank"}
