---
unique-page-id: 3571813
description: Steg 1 av 3 - Installera Marketo Solution i Dynamics (2013 On-Premises) - Marketo Docs - Produktdokumentation
title: Steg 1 av 3 - Installera Marketo Solution i Dynamics (On-Premises 2013)
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Steg 1 av 3: Installera Marketo Solution i Dynamics (2013 On-Premises) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Innan du kan synkronisera Microsoft Dynamics On-Premises och Marketo måste du först installera Marketo-lösningen i Dynamics.

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>Du måste ha [Driftsättning mot Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) med [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 eller 3.0 (ADFS) har konfigurerats. Obs! IFD-dokumentet laddas ned automatiskt när du klickar på länken.
>
>[Ladda ned Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) innan du börjar.

>[!NOTE]
>
>**Dynamics-administratörsbehörigheter krävs.**
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in **Dynamics**. Klicka på **Microsoft Dynamics CRM** nedrullningsbar meny och välj **Inställningar**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Under **Inställningar**, markera **Lösningar**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Klicka **Importera**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Klicka **Bläddra** och väljer [hämtad lösning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka **Nästa**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Visa lösningsinformationen och klicka på **Visa information om lösningspaket**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. När du är klar med kontrollen av all information klickar du på **Stäng**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Gå tillbaka till sidan Lösningsinformation, klicka på **Nästa**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Kontrollera att alternativet SDK är markerat. Klicka **Importera**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Vänta tills importen är klar.

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Hämta en loggfil (om du vill) och klicka på **Stäng**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management har slutförts med varning&quot;. Detta är helt förväntat.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management visas nu på **Alla lösningar** sida.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Välj Marketo och klicka **Publicera alla anpassningar**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Det var väl inte så illa? Kom igen, jag fortsätter gå dig genom resten.

>[!CAUTION]
>
>Om du inaktiverar någon av meddelandeprocesserna i Marketo SDK avbryts installationen!

>[!MORELIKETHIS]
>
>[Steg 2 av 3: Konfigurera Synkronisera användare för Marketo (lokal version 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)