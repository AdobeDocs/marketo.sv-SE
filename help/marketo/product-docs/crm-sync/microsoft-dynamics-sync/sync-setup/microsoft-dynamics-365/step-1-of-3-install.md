---
unique-page-id: 3571822
description: Steg 1 av 3 - Installera Marketo Solution (Online) - Marketo Docs - Produktdokumentation
title: Steg 1 av 3 -Installera Marketo-lösningen (online)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Steg 1 av 3: Installera Marketo-lösningen (online) {#step-of-install-the-marketo-solution-online}

Innan du kan synkronisera Microsoft Dynamics 365 och Marketo måste du först installera Marketo-lösningen i Dynamics. **Administratörsbehörigheter för Dynamics krävs.**

>[!CAUTION]
>
>* `Do not enable custom entity sync before the initial sync is completed. You will be notified via email once the initial sync is completed.`
>* Om Multi-Factor Authentication (MFA) är aktiverat för Dynamics Sync måste du inaktivera det för att Dynamics ska kunna synkroniseras korrekt med Marketo. Kontakta [Marketo Support](http://nation.marketo.com/community/support_solutions)om du vill ha mer information.

>



>[!NOTE]
>
>När du har synkroniserat Markto till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>[Ladda ned Marketo Lead Management Solution](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Logga in på ** [Microsoft Office 365](https://login.microsoftonline.com/) **.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Klicka på ![](assets/image2015-3-16-16-3a1-3a13.png)menyn och välj **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Klicka på ![](assets/image2015-5-13-10-3a5-3a8.png) menyn. I listrutan väljer du **Settings **och sedan **Solutions**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Klicka på **Importera.**

   ** ![](assets/image2015-3-19-8-3a34-3a8.png)

   **

1. Klicka på **Välj fil.** Välj den Marketo Lead Management-lösning du [laddat ned](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **Nästa**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Visa lösningsinformationen och klicka på **Visa information** om lösningspaketet.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. När du har kontrollerat alla detaljer klickar du på **Stäng**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Gå tillbaka till sidan Lösningsinformation och klicka på **Nästa**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Kontrollera att kryssrutan för SDK-alternativet är markerad. Klicka på **Importera**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

1. Vänta nu tills importen är klar. Ställ dig upp och sträck lite.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Klicka på **Stäng.**

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management klar med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo Lead Management visas nu i listan över lösningar.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Välj **Marketo Lead Management** och klicka på **Publish All Customizations.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Hög fem! Installationen är klar.

   >[!MORELIKETHIS]
   >
   >[Steg 2 av 3: Konfigurera Marketo Sync User i Dynamics](step-2-of-3-set-up.md)
