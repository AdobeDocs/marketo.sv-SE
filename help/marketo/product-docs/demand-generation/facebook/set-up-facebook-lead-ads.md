---
unique-page-id: 11379622
description: Konfigurera Facebook-annonser - Marketo Docs - Produktdokumentation
title: Konfigurera Facebook-annonser
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Konfigurera Facebook-annonser {#set-up-facebook-lead-ads}

Använd [Facebook Lead Ads](https://www.facebook.com/business/a/lead-ads) för att köra annonskampanjer på Facebook och generera leads för Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>**Tillgänglighet**
>
>Kontakta din Customer Success Manager om du vill lägga till Facebook-annonser i din instans.

1. Gå till Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **LaunchPoint**, klicka på **Nytt,** och välj **Ny tjänst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange ett **visningsnamn** för tjänsten, välj tjänsten **Facebook Lead Ads** i listrutan och klicka på **Skapa**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Öppna en ny flik i samma webbläsare och gå till [www.facebook.com.](http://www.facebook.com.) Logga in på Facebook med det konto du vill använda för integreringen.

   >[!NOTE]
   >
   >Facebook-kontot måste ha tillgång till alla Facebook-affärssidor som du vill hämta leads från.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. När du har loggat in på Facebook går du tillbaka till Marketo och klickar på **Auktorisera**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Om du uppmanas till det klickar du på **OK** för att godkänna Marketo-appinstallationen till Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du kommer att märka att du nu är auktoriserad. Klicka på **Nästa**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Markera den eller de sidor som du vill att Marketska ska hämta Facebook-annonser från och klicka på **Nästa**.

   >[!TIP]
   >
   >Om du inte ser någon sida som du väntar dig ska du kontrollera att det Facebook-konto som används för att autentisera läggs till på sidan på Facebook och försöka igen.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Om du vill acceptera standardfältmappningar från Facebook till Marketo klickar du bara på **Skapa**.

   >[!TIP]
   >
   >Genom att ändra mappningarna kan du anpassa var informationen om annonser för lead lagras i Marketo. Du kan även [hämta data från anpassade frågor för Lead Ads](set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo stöder inte mappning av två Facebook-fält till ett enskilt Marketo-fält, endast 1 till 1. Om du mappar 2 till 1 kan leads misslyckas med att gå in i Marketo-systemet.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   Snyggt gjort! Leads börjar flöda mot Marketo när ni kör framgångsrika Facebook-annonskampanjer.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Använd filter och utlösare för annonsering av leads i en smart kampanj](use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Mappa anpassade fält till markering](set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)

>



