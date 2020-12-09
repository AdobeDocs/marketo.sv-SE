---
unique-page-id: 3571813
description: Steg 1 av 3 - Installera Marketo Solution i Dynamics (2013 On-Premises) - Marketo Docs - Produktdokumentation
title: Steg 1 av 3 - Installera Marketo-lösningen i Dynamics (2013 On-Premises)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Steg 1 av 3: Installera Marketo-lösningen i Dynamics (On-Premises 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Innan du kan synkronisera Microsoft Dynamics On-Premises och Marketo måste du först installera Marketo-lösningen i Dynamics.

>[!NOTE]
>
>När du har synkroniserat Markto till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>IFD ( [Internet Facing Deployment](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) ) måste vara konfigurerat med [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 eller 3.0 (ADFS). Obs! IFD-dokumentet laddas ned automatiskt när du klickar på länken.
>
>[Ladda ned Marketo-lösningen](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) innan du börjar.

>[!NOTE]
>
>**Administratörsbehörigheter för Dynamics krävs.**
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in i **Dynamics**. Klicka på listrutan **Microsoft Dynamics CRM** och välj **INSTÄLLNINGAR**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Under **INSTÄLLNINGAR** väljer du **LÖSNINGAR**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Klicka på **Importera**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Klicka på **Bläddra** och välj den [hämtade lösningen](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **Nästa**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Visa lösningsinformationen och klicka på **Visa information** om lösningspaketet.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. När du har kontrollerat alla detaljer klickar du på **Stäng**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Gå tillbaka till sidan Lösningsinformation och klicka på **Nästa**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Kontrollera att alternativet SDK är markerat. Klicka på **Importera**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Vänta tills importen är klar.

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Hämta en loggfil (om du vill) och klicka på **Stäng**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management klar med varning&quot;. Detta är helt förväntat.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management visas nu på sidan **Alla lösningar** .

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Välj Marketo-lösningen och klicka på **Publicera alla anpassningar**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Det var väl inte så illa? Kom igen, jag fortsätter gå dig genom resten.

>[!CAUTION]
>
>Om du inaktiverar någon av Marketo SDK-meddelandeprocesserna avbryts installationen!

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Steg 2 av 3: Konfigurera Synkronisera användare för Marketo (lokal 2013)](step-2-of-3-configure.md)

>



