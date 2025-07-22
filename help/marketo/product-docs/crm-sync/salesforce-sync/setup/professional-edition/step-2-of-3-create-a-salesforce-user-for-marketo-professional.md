---
unique-page-id: 3571797
description: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Professional) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Professional)
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Steg 2 av 3: Skapa en [!DNL Salesforce]-användare för Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Dessa steg måste utföras av en Salesforce-administratör.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

I den här artikeln anpassar du fältbehörigheter med sidlayouten [!DNL Salesforce] och skapar en Marketo-[!DNL Salesforce]-synkroniseringsanvändare.

## Ange sidlayout {#set-page-layouts}

[!DNL Salesforce] Professional anger tillgänglighet på fältnivå med sidlayouter, till skillnad från [!DNL Salesforce] Enterprise/Unlimited&#39;s Profiles. Om du följer de här stegen kan Marketo synkroniseringsanvändare uppdatera anpassade fält.

1. Skriv [!UICONTROL page layouts] i navigeringsfältet utan att trycka på **[!UICONTROL Enter]** och klicka **[!UICONTROL Page Layout]** under **[!UICONTROL Leads]**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Klicka på **[!UICONTROL Edit]** bredvid Leadlayout.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Klicka och dra en ny **[!UICONTROL Section]** till sidlayouten.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Ange Marketo för **[!UICONTROL Section Name]** och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Klicka och dra fältet **[!UICONTROL Acquisition Date]** till avsnittet **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Upprepa ovanstående steg för följande fält:

   * [!UICONTROL Acquisition Program]
   * [!UICONTROL Acquisition Program Id]
   * [!UICONTROL Email Opt Out]
   * [!UICONTROL Inferred City]
   * [!UICONTROL Inferred Company]
   * [!UICONTROL Inferred Country]
   * [!UICONTROL Inferred Metropolitan Area]
   * [!UICONTROL Inferred Phone Area Code]
   * [!UICONTROL Inferred Postal Code]
   * [!UICONTROL Inferred State Region]
   * [!UICONTROL Lead Score]
   * [!UICONTROL Original Referrer]
   * [!UICONTROL Original Search Engine]
   * [!UICONTROL Original Search Phrase]
   * [!UICONTROL Original Source Info]
   * [!UICONTROL Original Source Type]

   >[!NOTE]
   >
   >Dessa fält måste finnas i sidlayouten så att Marketo kan läsa/skriva till dem.

   >[!TIP]
   >
   >Skapa två kolumner för fälten genom att dra nedåt till höger på sidan. Du kan flytta fält från den ena sidan till den andra om du vill balansera kolumnlängden.

1. Klicka på **[!UICONTROL Save]** när du är klar med att lägga till fält.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Upprepa alla ovanstående steg för Salesforce **[!UICONTROL Contact Page Layout]**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Kom ihåg att klicka på **[!UICONTROL Save]** när du är klar med **[!UICONTROL Contact Page Layout]**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Kontrollera att fältet **[!UICONTROL All-Day Event]** har lagts till i **[!UICONTROL Event Page Layout]**.

## Skapa synkroniserad användare {#create-sync-user}

Marketo kräver autentiseringsuppgifter för åtkomst till [!DNL Salesforce]. Detta görs bäst med en dedikerad användare som skapats med stegen nedan.

>[!NOTE]
>
>Om din organisation inte har några ytterligare Salesforce-licenser kan du använda en befintlig Marketing-användare med systemadministratörsprofilen.

1. Ange&quot;användare&quot; i navigeringsfältet och klicka på **[!UICONTROL Users]** under **[!UICONTROL Manage Users]**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Klicka på **[!UICONTROL New User]**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Fyll i de obligatoriska fälten, markera **[!UICONTROL User License: Salesforce]**, ange **[!UICONTROL Profile: System Administrator]**, kontrollera **[!UICONTROL Marketing User]** och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Kontrollera att den e-postadress du anger är giltig. Du måste logga in som synkroniseringsanvändare för att återställa lösenordet.

Underbar! Nu har du ett konto som Marketo kan använda för att ansluta till [!DNL Salesforce]. Låt oss göra det.

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Marketo och Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
