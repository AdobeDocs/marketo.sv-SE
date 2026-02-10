---
unique-page-id: 12976798
description: Konfigurera LinkedIn Lead Gen Forms - Marketo Docs - produktdokumentation
title: Konfigurera LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 0e164542f45045f5259b2e9c068bd3bade150656
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Konfigurera LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Använd LinkedIn Lead Gen Forms för att köra annonskampanjer i LinkedIn och generera leads för Marketo.

>[!NOTE]
>
>* **Administratörsbehörigheter krävs**
>
>* När du skapar LinkedIn Lead Gen-formulär ska du kontrollera att formulärnamnet inte bara innehåller numeriska tecken. Formulärnamnet måste vara antingen alfabetiskt eller alfanumeriskt.
>
>* En LinkedIn-lead kommer inte till Marketo Engage om den matchar en befintlig personpost i Marketo som är kopplad till en företagspost som skapats med företags-API:er, och Marketo-prenumerationen inte är ansluten till någon CRM.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/set-up-linkedin-lead-gen-forms-1.png)

1. Gå till **[!UICONTROL LaunchPoint]**, klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Service]**.

   ![](assets/set-up-linkedin-lead-gen-forms-2.png)

1. Ange ett _visningsnamn_ för tjänsten, välj tjänsten **[!UICONTROL LinkedIn Lead Gen]** i listrutan och klicka på **[!UICONTROL Next]**.

   ![](assets/set-up-linkedin-lead-gen-forms-3.png)

1. Marketo öppnar en ny flik i samma webbläsare till [linkedin.com](https://www.linkedin.com){target="_blank"}. Logga in på LinkedIn med det konto som du vill använda för integreringen.

   >[!NOTE]
   >
   >LinkedIn-kontot behöver tillgång till alla LinkedIn Business-konton som du skapar sponsrade kampanjer för.

   ![](assets/set-up-linkedin-lead-gen-forms-4.png)

1. När du har loggat in på LinkedIn går du tillbaka till Marketo och klickar på **[!UICONTROL Authorize]**.

   ![](assets/set-up-linkedin-lead-gen-forms-5.png)

1. När du uppmanas till det klickar du på **[!UICONTROL Allow]** för att godkänna Marketo-programinstallationen i LinkedIn.

   ![](assets/set-up-linkedin-lead-gen-forms-6.png)

1. Du kommer att märka att du nu är auktoriserad. Klicka på **[!UICONTROL Next]**.

   ![](assets/set-up-linkedin-lead-gen-forms-7.png)

   >[!CAUTION]
   >
   >Tjänsten upphör automatiskt ett år efter auktoriseringen. Klicka bara på **[!UICONTROL Re-Authorize]** om du vill återfå åtkomst. Du kan behöva ange ditt LinkedIn-lösenord igen, beroende på inställningarna i webbläsaren.

1. Markera det/de konton du vill att LinkedIn-lead Gen ska komma till Marketo från och klicka på **[!UICONTROL Next]**.

   >[!TIP]
   >
   >Om du inte ser de företagskonton som du förväntar dig ska du se till att användarens LinkedIn-konto som auktoriseras har Lead Gen Form Manager-behörigheter till företagskontot i LinkedIn.

   ![](assets/set-up-linkedin-lead-gen-forms-8.png)

1. Om du vill acceptera standardfältkopplingar från LinkedIn till Marketo klickar du bara på **[!UICONTROL Create]**. Om du vill ändra standardfältmappningen, ta bort en fältmappning eller lägga till en ny fältmappning, kan du göra detta per fält via modalen nedan.

   >[!CAUTION]
   >
   >Marketo stöder mappning av två LinkedIn-fält till ett enda Marketo-fält, _, men bara när_ de två LinkedIn-fälten inte finns i samma formulär. Om du mappar två fält från samma LinkedIn-formulär till ett enda Marketo-fält kan det hända att ingen kan komma att ange din Marketo-databas.

   ![](assets/set-up-linkedin-lead-gen-forms-9.png)

   >[!NOTE]
   >
   >Endast LinkedIn-fält som redan har sparats i en [formulärmall](https://www.linkedin.com/help/lms/answer/79634){target="_blank"} i LinkedIn Campaign Manager visas som LinkedIn-fält som kan mappas till Marketo-fält.

   ![](assets/set-up-linkedin-lead-gen-forms-10.png)

Snyggt gjort! Personer som skickar in LinkedIn-formulär för Lead Gen börjar flöda in i Marketo när ni kör framgångsrika kampanjer på LinkedIn-sidan.

>[!NOTE]
>
>Du kan bara auktorisera ett enstaka LinkedIn-användarkonto. Om du har flera företagskonton som du vill länka till Marketo måste du se till att användarens LinkedIn-konto som auktoriseras har Lead Gen Form Manager-behörigheter till företagskontot i LinkedIn.

>[!MORELIKETHIS]
>
>[Använd LinkedIn-formulärfilter och utlösare för lead-generering i en smart kampanj](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
