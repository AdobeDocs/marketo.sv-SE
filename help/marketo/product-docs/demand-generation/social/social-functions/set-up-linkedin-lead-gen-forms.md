---
unique-page-id: 12976798
description: Konfigurera LinkedIn Lead Gen Forms - Marketo Docs - Produktdokumentation
title: Konfigurera LinkedIn Lead Gen Forms
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Konfigurera LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Använd LinkedIn Lead Gen Forms för att köra annonskampanjer i LinkedIn och generera leads för Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **LaunchPoint**, klicka på **Ny** och välj **Ny tjänst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange ett **visningsnamn** för tjänsten, välj tjänsten **LinkedIn Lead Gen **i listrutan och klicka på **Nästa**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo öppnar en ny flik i samma webbläsare till [www.linkedin.com](http://www.linkedin.com). Logga in på LinkedIn med det konto som du vill använda för integreringen.

   >[!NOTE]
   >
   >LinkedIn-kontot behöver tillgång till alla LinkedIn Business-konton som du skapar sponsrade kampanjer för.

   ![](assets/linkedin-login.png)

1. När du har loggat in på LinkedIn går du tillbaka till Marketo och klickar på **Authorize**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. När du uppmanas till det klickar du på **Allow **för att godkänna Marketo-appinstallationen i LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Du kommer att märka att du nu är auktoriserad. Klicka på **Nästa**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Tjänsten upphör automatiskt ett år efter auktoriseringen. Klicka bara på **Återauktorisera** om du vill återfå åtkomsten. Du kan behöva ange ditt LinkedIn-lösenord igen, beroende på inställningarna i webbläsaren.

1. Markera det eller de konton som du vill att LinkedIn-lead-Gen ska komma till Marketo från och klicka på **Nästa**.

   >[!TIP]
   >
   >Om du inte ser de företagskonton som du förväntar dig ska du se till att användarens LinkedIn-konto som auktoriseras har Lead Gen Form Manager-behörigheter till företagskontot i LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Om du vill acceptera standardfältkopplingar för LinkedIn till Marketo klickar du bara på **Skapa**. Om du vill ändra standardfältmappningen, ta bort en fältmappning eller lägga till en ny fältmappning, kan du göra detta per fält via modalen nedan.

   >[!CAUTION]
   >
   >Marketo stöder mappning av två LinkedIn-fält till ett enda Marketo-fält, **men endast när** de två LinkedIn-fälten inte finns i samma formulär. Om du mappar två fält från samma LinkedIn-formulär till ett enda Marketo-fält kan det hända att ingen kan ange din Marketo-databas.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Endast LinkedIn-fält som redan har sparats i en [formulärmall](https://www.linkedin.com/help/lms/answer/79634) i LinkedIn Campaign Manager visas som LinkedIn-fält som kan mappas till Marketo-fält.

   ![](assets/linkedin-installed-services.png)

Snyggt gjort! Personer som skickar in LinkedIn Lead Gen-formulär börjar flöda in på Marketo när ni kör framgångsrika kampanjer på LinkedIn-sidan.

>[!NOTE]
>
>Du kan bara auktorisera ett enstaka LinkedIn-användarkonto. Om du har flera företagskonton som du vill länka till Marketo kontrollerar du att användarens LinkedIn-konto som auktoriseras har Lead Gen Form Manager-behörigheter till företagskontot i LinkedIn.

>[!MORELIKETHIS]
>
>* [Använd LinkedIn-formulärfilter och utlösare för lead-generering i en smart kampanj](use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)

>



