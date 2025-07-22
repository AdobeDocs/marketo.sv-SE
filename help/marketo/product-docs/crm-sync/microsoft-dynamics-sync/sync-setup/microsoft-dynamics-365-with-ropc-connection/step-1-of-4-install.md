---
description: Steg 1 av 4 - Installera Marketo Solution med Resource Owner Password Control Connection - Marketo Docs - Product Documentation
title: Steg 1 av 4 - Installera Marketo Solution med Resource Owner Password Control Connection
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 1%

---

# Steg 1 av 4: Installera Marketo Solution med Resource Owner Password Control Connection {#step-1-of-4-install-the-marketo-solution-ropc}

Innan du kan synkronisera [!DNL Microsoft Dynamics] 365 och Marketo måste du först installera Marketo-lösningen i [!DNL Dynamics]. **[!DNL Dynamics]Administratörsbehörigheter krävs.**

>[!CAUTION]
>
>* Aktivera inte anpassad entitetssynkronisering innan den inledande synkroniseringen har slutförts. Du meddelas via e-post när den första synkroniseringen är klar.
>* Om Multi-Factor Authentication (MFA) är aktiverat för din [!DNL Dynamics]-synkronisering måste du inaktivera det för att [!DNL Dynamics] ska kunna synkronisera korrekt med Marketo. Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) om du vill ha mer information.

>[!NOTE]
>
>När du har synkroniserat Marketo till en CRM kan du inte utföra en ny synkronisering utan att ersätta instansen.

>[!PREREQUISITES]
>
>[Hämta Marketo Lead Management Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Logga in på **[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Klicka på menyn ![](assets/image2015-3-16-16-3a1-3a13.png) och välj **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Klicka på menyn ![](assets/image2015-5-13-10-3a5-3a8.png). I listrutan väljer du **[!UICONTROL Settings]** och sedan **[!UICONTROL Solutions]**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Klicka på **[!UICONTROL Choose File]**. Välj den Marketo Lead Management-lösning som du [hämtade](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Visa lösningsinformationen och klicka på **[!UICONTROL View solution package details]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. När du har kontrollerat alla detaljer klickar du på **[!UICONTROL Close]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicka på **[!UICONTROL Next]** på sidan Lösningsinformation igen.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Kontrollera att kryssrutan för alternativet SDK är markerad. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Du måste aktivera popup-fönster i webbläsaren för att slutföra installationen.

1. Vänta nu tills importen är klar. Ställ dig upp och sträck lite.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Klicka på **[!UICONTROL Close]**.

   >[!NOTE]
   >
   >Du kan se ett meddelande med texten&quot;Marketo Lead Management har slutförts med varning&quot;. Detta är helt förväntat.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. &quot;Marketo Lead Management&quot; visas nu i listan över lösningar.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Markera **[!UICONTROL Marketo Lead Management]** och klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Snyggt jobbat! Installationen är klar.

   >[!MORELIKETHIS]
   >
   >[Steg 2 av 4: Konfigurera Marketo-lösningen med Resursägarens lösenordskontrollanslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
