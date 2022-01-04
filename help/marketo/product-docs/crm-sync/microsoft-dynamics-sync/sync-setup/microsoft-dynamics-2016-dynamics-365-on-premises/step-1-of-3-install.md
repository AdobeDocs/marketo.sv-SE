---
description: Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises 1 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 1 of 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Steg 1 av 3: Konfigurera Synkronisera användare för Marketo (lokal version 2016 /Dynamics 365) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Innan du kan synkronisera Microsoft Dynamics 2016 On-Prem/Dynamics 365 med Marketo måste du först installera Marketo-lösningen i Dynamics.

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte synkronisera en ny CRM till den befintliga Marketo-instansen.

>[!PREREQUISITES]
>
>Om du använder Microsoft Dynamics On-Premise måste du ha [Driftsättning mot Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) med [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) har konfigurerats. Obs! IFD-dokumentet laddas ned automatiskt när du klickar på länken.
>
>[Ladda ned Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) innan du börjar.

>[!NOTE]
>
>**Dynamics-administratörsbehörigheter krävs.**
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in på **Dynamics.** Klicka på **Microsoft Dynamics CRM** nedrullningsbar meny och välj **Inställningar**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Under **Inställningar**, markera **Lösningar**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicka **Importera**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicka **Bläddra** och välj den lösning du behöver [nedladdad](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka **Nästa**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visa lösningsinformationen och klicka på **Visa information om lösningspaket**.

   ![](assets/image2015-11-18-11-12-8.png)

1. När du är klar med kontrollen av all information klickar du på **Stäng**.

   ![](assets/step6.png)

1. Gå tillbaka till sidan Lösningsinformation, klicka på **Nästa**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Kontrollera att kryssrutan för SDK-alternativet är markerad. Klicka **Importera**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Vänta tills importen är klar.

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Hämta en loggfil (om du vill) och klicka på **Stäng**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management har slutförts med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management visas nu på **Alla lösningar** sida.

   ![](assets/image2015-3-19-8-40-38.png)

1. Välj Marketo och klicka **Publicera alla anpassningar**.

   ![](assets/image2015-3-19-8-41-21.png)

   Hög fem! Installationen är klar.

   >[!CAUTION]
   >
   >Om du inaktiverar någon av meddelandeprocesserna i Marketo SDK avbryts installationen!

   >[!MORELIKETHIS]
   >
   >[Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 2 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
