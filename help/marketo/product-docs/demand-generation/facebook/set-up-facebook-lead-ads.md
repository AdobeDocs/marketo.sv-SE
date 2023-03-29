---
unique-page-id: 11379622
description: Konfigurera Facebook Lead Ads - Marketo Docs - produktdokumentation
title: Konfigurera Facebook Lead Ads
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Konfigurera Facebook Lead Ads {#set-up-facebook-lead-ads}

Använd [Facebook Lead Ads](https://www.facebook.com/business/a/lead-ads) för att köra annonskampanjer i Facebook och generera leads för Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!AVAILABILITY]
>
>Om du vill lägga till Facebook Lead Ads i din instans kontaktar du kontoteamet på Adobe (din kontoansvarige).

1. Gå till Marketo **Administratör**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **LaunchPoint**, klicka på **Nytt,** och markera **Ny tjänst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange **Visningsnamn** för tjänsten väljer du **Facebook Lead Ads** i listrutan och klicka på **Skapa**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Öppna en ny flik i samma webbläsare och gå till [facebook.com](https://www.facebook.com). Logga in på Facebook med det konto du vill använda för integreringen.

   >[!NOTE]
   >
   >Facebook-kontot måste ha tillgång till alla Facebook företagssidor som du vill hämta leads från.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. När du har loggat in på Facebook går du tillbaka till Marketo och klickar på **Auktorisera**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Om du uppmanas till det klickar du på **OK** för att acceptera Marketo-appinstallationen i Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du kommer att märka att du nu är auktoriserad. Klicka **Nästa**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Markera de sidor du vill att Marketo ska hämta Facebook Lead Ads från och klicka på **Nästa**.

   >[!TIP]
   >
   >Om du inte ser någon sida som du väntar dig ser du till att det Facebook-konto som används för att autentisera läggs till på sidan i Facebook och försöker igen.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Om du vill acceptera standardfältkopplingar från Facebook till Marketo klickar du bara på **Skapa**.

   >[!TIP]
   >
   >Genom att ändra mappningarna kan du anpassa var informationen om annonser för leads lagras i Marketo. Du kan också [hämta in data från Lead Ads - anpassade frågor](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo stöder inte mappning av två Facebook-fält till ett enda Marketo-fält, endast 1 till 1. Om du mappar 2 till 1 kan leads misslyckas med att ansluta till Marketo.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   Snyggt gjort! Leads kommer att börja flöda in i Marketo när ni kör framgångsrika Facebook Lead Ad-kampanjer.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Tilldela/ta bort behörigheter i Leads Access Manager (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Använd filter och utlösare för annonsering av leads i en smart kampanj](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Mappa anpassade fält till Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)

