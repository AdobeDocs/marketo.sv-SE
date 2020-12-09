---
unique-page-id: 3571827
description: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---


# Steg 2 av 3: Konfigurera Marketo Sync User i Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Vi börjar med att skapa ett användarkonto.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo-lösningen (online)](step-1-of-3-install.md)

## Skapa en ny användare {#create-a-new-user}

1. Logga in i Dynamics. Klicka på ikonen Inställningar och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på** Inställningar** och välj **Dokumentskydd**.

   ![](assets/two.png)

1. Klicka på **Användare**.

   ![](assets/three.png)

1. Klicka på **Ny.**

   ![](assets/four.png)

1. Klicka på **Lägg till och licensiera användare** i det nya fönstret.

   ![](assets/five.png)

1. En ny flik öppnas. Klicka på **Admin** överst på sidan.

   ![](assets/six.png)

1. En annan ny flik öppnas. Klicka på **Lägg till en användare**.

   ![](assets/seven.png)

1. Ange all information. När du är klar klickar du på **Lägg till**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Det här namnet måste vara en dedikerad synkroniseringsanvändare och inte en befintlig CRM-användares konto. Det behöver inte vara en faktisk e-postadress.

1. Ange e-postadressen som ska ta emot inloggningsuppgifterna för den nya användaren och klicka på **Skicka e-post och stäng**.

   ![](assets/nine.png)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo-synkroniseringsanvändarrollen till Marketför att synkronisera användare. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar Marketo finns i [Upgrade Marketo Solution för Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Gå tillbaka till fliken Aktiverade användare och uppdatera användarlistan.

   ![](assets/ten.png)

1. Hovra bredvid den nyligen skapade Marketo Sync-användaren så visas en kryssruta. Klicka för att markera den.

   ![](assets/eleven.png)

1. Klicka på **Hantera roller**.

   ![](assets/twelve.png)

1. Markera **Marketo Sync User** och klicka på **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Uppdateringar som görs i CRM av Synkronisera användare synkroniseras **inte** tillbaka till Marketo.

## Konfigurera Marketo-lösning {#configure-marketo-solution}

Nästan klart! Allt vi har kvar är att informera Marketo Solution om den nya användaren som har skapats.

1. Gå tillbaka till avsnittet Avancerade inställningar och klicka på ![](assets/image2015-5-13-15-3a49-3a19.png)ikonen bredvid Inställningar och välj **Marketo Config**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Uppdatera sidan om du inte ser **Marketo Config** på menyn Inställningar. Om det inte fungerar kan du försöka [publicera Marketo-lösningen](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) [](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) igen eller logga ut och in igen.

1. Klicka på **Standard**.

   ![](assets/fifteen.png)

1. Klicka på sökknappen i fältet **Marketo-användare** och välj den synkroniseringsanvändare du skapade.

   ![](assets/sixteen.png)

1. Klicka på ![](assets/image2015-3-13-15-3a10-3a11.png)ikonen längst ned till höger för att spara ändringarna.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicka på **X** i det övre högra hörnet för att stänga skärmen.

   ![](assets/seventeen.png)

1. Klicka på ![](assets/image2015-5-13-15-3a49-3a19-1.png)ikonen bredvid Inställningar och välj **Lösningar**.

   ![](assets/eighteen.png)

1. Klicka på knappen **Publicera alla anpassningar** .

   ![](assets/nineteen.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

    * Om du vill begränsa antalet poster som du synkroniserar [konfigurera ett anpassat synkroniseringsfilter](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
    * Kör processen [Validera Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
    * Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!NOTE]
>
>**Relaterade artiklar**
>
>
>[Steg 3 av 3: Anslut Microsoft Dynamics med Marketo (online)](step-3-of-3-connect.md)
