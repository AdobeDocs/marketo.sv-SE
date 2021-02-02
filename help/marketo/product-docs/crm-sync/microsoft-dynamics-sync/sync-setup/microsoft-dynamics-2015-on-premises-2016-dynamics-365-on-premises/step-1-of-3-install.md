---
unique-page-id: 7504736
description: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 1 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 1 of 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Steg 1 av 3: Konfigurera Synkronisera användare för Marketo (On-Prem 2015 och 2016 365 On-Prem) {#step-of-configure-sync-user-for-marketo-on-premises-and-365}

Innan du kan synkronisera Microsoft Dynamics 2015 On-Premises eller 2016 (Dynamics 365) med Marketo måste du först installera Marketo-lösningen i Dynamics.

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte synkronisera en ny CRM till den befintliga Marketo-instansen.

>[!PREREQUISITES]
>
>Om du använder Microsoft Dynamics On-Premise måste du ha [Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) med [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) konfigurerat. Obs! IFD-dokumentet laddas ned automatiskt när du klickar på länken.
>
>[Ladda ned Marketo Lead Management ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solution innan du börjar.

>[!NOTE]
>
>**Administratörsbehörigheter för Dynamics krävs.**
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in på **Dynamics.** Klicka på listrutan  **Microsoft Dynamics** CRM och välj  **Inställningar**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Under **Inställningar** väljer du **Lösningar**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicka på **Importera**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicka på **Bläddra** och välj den lösning du [hämtade](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **Nästa**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visa lösningsinformationen och klicka på **Visa information om lösningspaketet**.

   ![](assets/image2015-11-18-11-12-8.png)

1. När du är klar med att kontrollera all information klickar du på **Stäng**.

   ![](assets/step6.png)

1. Gå tillbaka till sidan Lösningsinformation och klicka på **Nästa**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Kontrollera att kryssrutan för SDK-alternativet är markerad. Klicka på **Importera**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Vänta tills importen är klar.

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Hämta en loggfil (om du vill) och klicka på **Stäng**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management klar med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management visas nu på sidan **Alla lösningar**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Välj Marketo-lösningen och klicka på **Publicera alla anpassningar**.

   ![](assets/image2015-3-19-8-41-21.png)

   Hög fem! Installationen är klar.

   >[!CAUTION]
   >
   >Om du inaktiverar någon av Marketo SDK-meddelandeprocesserna avbryts installationen!

   >[!MORELIKETHIS]
   >
   >[Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 2 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
