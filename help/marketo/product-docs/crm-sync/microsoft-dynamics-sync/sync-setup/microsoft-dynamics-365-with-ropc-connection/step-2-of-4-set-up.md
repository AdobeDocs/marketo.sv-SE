---
description: Steg 2 av 4 - Konfigurera Marketo Solution med Resource Owner Password Control Connection - Marketo Docs - Product Documentation
title: Steg 2 av 4 - Konfigurera Marketo Solution med Resource Owner Password Control Connection
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Steg 2 av 4: Konfigurera Marketo Solution med Resource Owner Password Control Connection {#step-2-of-4-set-up-the-marketo-solution-ropc}

Vi börjar med att skapa ett användarkonto.

>[!PREREQUISITES]
>
>[Steg 1 av 4: Installera Marketo-lösningen med Resursägarens lösenordskontrollanslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Skapa en ny användare {#create-a-new-user}

1. Logga in på [!DNL Dynamics]. Klicka på ikonen [!UICONTROL Settings] och välj **[!UICONTROL Advanced Settings]**.

   ![](assets/one.png)

1. Klicka på **[!UICONTROL Settings]** och välj **[!UICONTROL Security]**.

   ![](assets/two.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/three.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/four.png)

1. Klicka på **[!UICONTROL Add and License Users]** i det nya fönstret.

   ![](assets/five.png)

1. En ny flik öppnas. Klicka på **[!UICONTROL Admin]** överst på sidan.

   ![](assets/six.png)

1. En annan ny flik öppnas. Klicka på **[!UICONTROL Add a user]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >Synkroniseringsanvändaren bör ha läsbehörighet för Marketo Config.

1. Ange all information. När du är klar klickar du på **[!UICONTROL Add]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Det här namnet måste vara en dedikerad synkroniseringsanvändare och inte en befintlig CRM-användares konto. Det behöver inte vara en faktisk e-postadress.

1. Ange e-postadressen som ska ta emot inloggningsuppgifterna och klicka på **[!UICONTROL Send email and close]**.

   ![](assets/nine.png)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller för Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar Marketo finns i [Uppgradera Marketo-lösning för [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Språkinställningen för synkroniseringsanvändaren [ ska anges till engelska](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Gå tillbaka till fliken [!UICONTROL Enabled Users] och uppdatera användarlistan.

   ![](assets/ten.png)

1. Hovra bredvid den nya Marketo Sync-användaren så visas en kryssruta. Klicka för att markera den.

   ![](assets/eleven.png)

1. Klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/twelve.png)

1. Markera **[!UICONTROL Marketo Sync User]** och klicka på **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare _synkroniseras inte_ tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Allt vi har kvar är att informera Marketo Solution om den nya användaren som har skapats.

1. Gå tillbaka till avsnittet [!UICONTROL Advanced Settings], klicka på ikonen ![](assets/image2015-5-13-15-3a49-3a19.png) intill [!UICONTROL Settings] och välj **[!UICONTROL Marketo Config]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Uppdatera sidan om du inte ser **[!UICONTROL Marketo Config]** på menyn [!UICONTROL Settings]. Om det inte fungerar kan du försöka med att [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) igen eller logga ut och in igen.

1. Klicka på **[!UICONTROL Default]**.

   ![](assets/fifteen.png)

1. Klicka på sökknappen i fältet **[!UICONTROL Marketo User]** och välj den synkroniseringsanvändare du skapade.

   ![](assets/sixteen.png)

1. Klicka på ikonen ![](assets/image2015-3-13-15-3a10-3a11.png) längst ned till höger för att spara ändringarna.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicka på **X** i det övre högra hörnet för att stänga skärmen.

   ![](assets/seventeen.png)

1. Klicka på ikonen ![](assets/image2015-5-13-15-3a49-3a19-1.png) bredvid [!UICONTROL Settings] och välj **[!UICONTROL Solutions]**.

   ![](assets/eighteen.png)

1. Klicka på knappen **[!UICONTROL Publish All Customizations]**.

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Steg 3 av 4: Anslut Marketo-lösningen med Resursägarens lösenordskontrollanslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
