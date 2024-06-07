---
description: Överför ett Adobe Experience Platform-segment till en Marketo Static List - Marketo Docs - Product Documentation
title: Överför ett Adobe Experience Platform-segment till en Marketo Static List
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Överför ett Adobe Experience Platform-segment till en Marketo Static List {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Med den här funktionen kan du skicka segment som finns i din Adobe Experience Platform till Marketo Engage i form av en statisk lista.

>[!PREREQUISITES]
>
>* [Redigera API-rollen](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role){target="_blank"} för att säkerställa att den har **Skrivskyddad person** behörighet (finns i listrutan Åtkomst-API).
>* [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"} i Marketo.
>* Gå till **[!UICONTROL Admin]** > **[!UICONTROL Launchpoint]**. Sök efter namnet på den roll du just skapade och klicka på **[!UICONTROL View Details]**. Kopiera och spara informationen i **[!UICONTROL Client ID]** och **[!UICONTROL Client Secret]** som du kunde behöva det för steg 7.
>* Skapa en statisk lista i Marketo eller sök efter och välj en som du redan har skapat. Du behöver dess ID.

1. Logga in på [Adobe Experience Platform](https://experience.adobe.com/){target="_blank"}.

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Klicka på rutnätsikonen och välj **[!UICONTROL Experience Platform]**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Klicka på **[!UICONTROL Destinations]**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Klicka på **[!UICONTROL Catalog]**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Hitta plattan Marketo Engage och klicka **[!UICONTROL Activate]**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Klicka på **[!UICONTROL Configure New Destination]**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. Under Kontotyp väljer du alternativknappen Befintligt eller Nytt konto (i det här exemplet väljer vi **[!UICONTROL Existing Account]**). Klicka på ikonen Välj konto.

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Om du väljer Nytt konto kan du hitta ditt Munchkin-ID genom att gå till **[!UICONTROL Admin]** > **[!UICONTROL Munchkin]** (den ingår också i din Marketo-URL när du har loggat in). Klient-ID/hemlighet som du bör ha från att följa de krav som anges högst upp i den här artikeln.

1. Välj destinationskontot och klicka på **[!UICONTROL Select]**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Ange ett mål **[!UICONTROL Name]** och en valfri beskrivning. Klicka på listrutan Skapa person och välj&quot;Matcha befintliga Marketo-personer och skapa saknade personer i Marketo&quot; _eller_ &quot;Matcha endast befintliga Marketo-användare&quot; (i det här exemplet väljer vi den första). Du måste också välja en **[!UICONTROL Workspace]**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Om du väljer&quot;Matcha endast befintliga Marketo-användare&quot; behöver du bara mappa e-postmeddelandet och/eller ECID så att du kan hoppa över steg 13-16.

1. Det här avsnittet är valfritt. Klicka **[!UICONTROL Create]** att hoppa över.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Markera målet som du skapade och klicka på **[!UICONTROL Next]**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Välj det segment som du vill skicka till Marketo och klicka på **[!UICONTROL Next]**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Om du väljer flera segment måste du mappa varje segment till en angiven statisk lista på fliken Segmentschema.

   >[!IMPORTANT]
   >
   >När ett segment har aktiverats för första gången på Marketo-målet kan de bakåtfyllnadsprofiler som redan fanns i segmentet innan Marketo-målaktiveringen aktiveras _upp till 24 timmar_. Framöver kommer profiler som läggs till i segmentet att läggas till i Marketo direkt.

1. Klicka på **[!UICONTROL Add New Mapping]**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Klicka på mappningsikonen.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Välj önskade attribut och klicka på **[!UICONTROL Select]**. I det här exemplet väljer vi förnamn, efternamn och e-postadress.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >Du kan mappa attribut från Experience Platform till attribut som din organisation har åtkomst till i Marketo Engage. Använd [Beskriv API-begäran](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database#describe){target="_blank"} för att hämta attributfält som din organisation har åtkomst till.

1. Mappa efternamn och företagsnamn genom att klicka på **[!UICONTROL Add New Mapping]** och upprepa steg 15 två gånger genom att välja **[!UICONTROL lastName]** och sedan **[!UICONTROL companyName]**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Nu är det dags att mappa e-postadressen. Klicka **[!UICONTROL Add New Mapping]** igen.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Klicka på mappningsikonen.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Klicka på alternativknappen Välj identitetsnamnområde och välj **[!UICONTROL Email]** och sedan klicka **[!UICONTROL Select]**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Mappa e-post och/eller ECID från **[!UICONTROL Identity Namespace]** -fliken är det viktigaste att göra för att säkerställa att personen matchas i Marketo. Mappning via e-post ger högsta matchningsfrekvens.

1. Nu är det dags att välja källfälten. Klicka på markörikonen för e-post.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Klicka på alternativknappen Välj identitetsnamnutrymme, sök efter och markera **[!UICONTROL Email]** och sedan klicka **[!UICONTROL Select]**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Om du vill välja källfältet för företagsnamnet klickar du på markörikonen på raden.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Låt alternativknappen Välj attribut vara markerad. Sök efter&quot;företag&quot; och välj **[!UICONTROL companyName]** och sedan klicka **[!UICONTROL Select]**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Mappa källfälten för Efternamn och Förnamn genom att klicka på markörikonen för varje och upprepa steg 23 två gånger. Välj **[!UICONTROL lastName]** och sedan **[!UICONTROL firstName]**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Granska ändringarna och klicka på **[!UICONTROL Finish]**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
