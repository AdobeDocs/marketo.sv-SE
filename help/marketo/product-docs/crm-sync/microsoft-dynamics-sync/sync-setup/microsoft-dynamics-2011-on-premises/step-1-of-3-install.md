---
unique-page-id: 3571805
description: Steg 1 av 3 - Installera Marketo Solution (2011 On-Premises) - Marketo Docs - Produktdokumentation
title: Steg 1 av 3 - Installera Marketo Solution (2011 On-Premises)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Steg 1 av 3: Installera Marketo-lösningen (2011 On-Premises) {#step-of-install-the-marketo-solution-on-premises}

Innan du kan synkronisera Microsoft Dynamics On-Premises och Marketo måste du först installera Marketo-lösningen i Dynamics.

>[!NOTE]
>
>När du har synkroniserat Markto till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>Du måste ha [Internet Facing Deployment](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) med [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 eller 3.0 (ADFS) konfigurerat. **Obs**: IFD-dokumentet laddas ned automatiskt när du klickar på länken.
>
>[Ladda ned Marketo Lead Management ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solution innan du börjar.

>[!NOTE]
>
>**Administratörsbehörigheter för Dynamics krävs.**
>
>Du behöver administratörsbehörighet för CRM för att kunna utföra den här synkroniseringen.

1. Logga in på **Dynamics** och välj **Inställningar** längst ned på den vänstra menyn.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Välj **Lösningar** i trädet.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Klicka på **Importera**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Klicka på **Bläddra**. Välj den Marketo Lead Management-lösning som du [har hämtat](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **Nästa**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Visa lösningsinformationen och klicka på **Visa information om lösningspaketet**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. När du är klar med att kontrollera all information klickar du på **Stäng**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Gå tillbaka till sidan Lösningsinformation och klicka på **Nästa**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Kontrollera att kryssrutan för SDK-meddelandealternativet är markerad. Klicka på **Nästa**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

1. Vänta nu tills importen är klar. Ställ dig upp och sträck lite.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Klicka på **Stäng**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management klar med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management visas nu på sidan **Alla lösningar**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Välj Marketo Lead Management och klicka på **Publicera alla anpassningar.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

Det var väl inte så illa? Kom igen, jag fortsätter gå dig genom resten.

>[!CAUTION]
>
>Om du inaktiverar någon av Marketo SDK-meddelandeprocesserna avbryts installationen!

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Steg 2 av 3: Konfigurera Marketo-synkronisering av användare i Dynamics (lokal 2011)](step-2-of-3-set-up.md)
