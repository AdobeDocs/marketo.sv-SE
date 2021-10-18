---
unique-page-id: 12976798
description: Konfigurera LinkedIn Lead Gen Forms - Marketo Docs - produktdokumentation
title: Konfigurera LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Konfigurera LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Använd LinkedIn Lead Gen Forms för att köra annonskampanjer i LinkedIn och generera leads för Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till Marketo **Administratör**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **LaunchPoint**, klicka på **Nytt** och markera **Ny tjänst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange **Visningsnamn** för tjänsten väljer du **linkedIn Lead Gen** i listrutan och klicka på **Nästa**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo öppnar en ny flik i samma webbläsare för att [linkedin.com](https://www.linkedin.com). Logga in på LinkedIn med det konto du vill använda för integreringen.

   >[!NOTE]
   >
   >LinkedIn-kontot behöver tillgång till alla LinkedIn Business-konton som du skapar sponsrade kampanjer för.

   ![](assets/linkedin-login.png)

1. När du har loggat in på LinkedIn går du tillbaka till Marketo och klickar på **Auktorisera**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Klicka på **Tillåt** för att acceptera Marketo-appinstallationen i LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Du kommer att märka att du nu är auktoriserad. Klicka **Nästa**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Tjänsten upphör automatiskt ett år efter auktoriseringen. Klicka bara på **Återauktorisera**. Du kan behöva ange ditt LinkedIn-lösenord igen, beroende på inställningarna för webbläsaren.

1. Välj det/de konton du vill att LinkedIn Lead Gen-leads ska komma till Marketo från och klicka på **Nästa**.

   >[!TIP]
   >
   >Om du inte ser de företagskonton du förväntar dig ska du se till att användarens LinkedIn-konto som auktoriseras har Lead Gen Form Manager-behörigheter till företagskontot i LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Om du vill acceptera standardfältkopplingar från LinkedIn till Marketo klickar du bara på **Skapa**. Om du vill ändra standardfältmappningen, ta bort en fältmappning eller lägga till en ny fältmappning, kan du göra detta per fält via modalen nedan.

   >[!CAUTION]
   >
   >Marketo har stöd för att mappa två LinkedIn-fält till ett Marketo-fält, **men bara när** de två LinkedIn-fälten inte finns i samma formulär. Om du mappar två fält från samma LinkedIn-formulär till ett enda Marketo-fält kan det hända att ingen kan ange Marketo-databasen.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Endast LinkedIn-fält som redan har sparats i en [formulärmall](https://www.linkedin.com/help/lms/answer/79634) i LinkedIn Campaign Manager visas som LinkedIn-fält som kan mappas till Marketo-fält.

   ![](assets/linkedin-installed-services.png)

Snyggt gjort! Personer som skickar in LinkedIn Lead Gen-formulär börjar flöda in i Marketo när ni genomför framgångsrika kampanjer på LinkedIn sida.

>[!NOTE]
>
>Du kan bara auktorisera ett LinkedIn-användarkonto. Om du har flera Business-konton som du vill länka till Marketo måste du se till att användarens LinkedIn-konto som auktoriseras har Lead Gen Form Manager-behörighet till företagskontot i LinkedIn.

>[!MORELIKETHIS]
>
>[Använd LinkedIn Lead Gen Form Filters and Triggers i en smart kampanj](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
