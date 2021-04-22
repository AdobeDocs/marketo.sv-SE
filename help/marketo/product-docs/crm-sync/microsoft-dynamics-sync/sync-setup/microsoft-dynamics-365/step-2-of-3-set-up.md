---
unique-page-id: 3571827
description: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Marketo Sync User i Dynamics
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Steg 2 av 3: Konfigurera Marketo Sync User i Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Vi börjar med att skapa ett användarkonto.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo-lösningen (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## Skapa en ny användare {#create-a-new-user}

1. Logga in i Dynamics. Klicka på ikonen Inställningar och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka på **Inställningar** och välj **Säkerhet**.

   ![](assets/two.png)

1. Klicka på **Användare**.

   ![](assets/three.png)

1. Klicka på **Nytt.**

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

1. Ange e-postmeddelandet som ska ta emot inloggningsuppgifterna för den nya användaren och klicka på **Skicka e-post och stäng**.

   ![](assets/nine.png)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar Marketo finns i [Uppgradera Marketo-lösning för Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Gå tillbaka till fliken Aktiverade användare och uppdatera användarlistan.

   ![](assets/ten.png)

1. Hovra bredvid den nya Marketo Sync-användaren så visas en kryssruta. Klicka för att markera den.

   ![](assets/eleven.png)

1. Klicka på **Hantera roller**.

   ![](assets/twelve.png)

1. Markera **Marketo Sync User** och klicka på **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Sync User kommer **inte** att synkroniseras tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Allt vi har kvar är att informera Marketo Solution om den nya användaren som har skapats.

1. Gå tillbaka till avsnittet Avancerade inställningar och klicka på ikonen ![](assets/image2015-5-13-15-3a49-3a19.png) bredvid Inställningar och välj **Marketo Config**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Uppdatera sidan om du inte ser **Marketo Config** på menyn Inställningar. Om det inte fungerar kan du försöka med att [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) igen eller logga ut och in igen.

1. Klicka på **Standard**.

   ![](assets/fifteen.png)

1. Klicka på sökknappen i fältet **Marketo-användare** och välj den synkroniseringsanvändare du skapade.

   ![](assets/sixteen.png)

1. Klicka på ikonen ![](assets/image2015-3-13-15-3a10-3a11.png) längst ned till höger för att spara ändringarna.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicka på **X** i det övre högra hörnet för att stänga skärmen.

   ![](assets/seventeen.png)

1. Klicka på ikonen ![](assets/image2015-5-13-15-3a49-3a19-1.png) bredvid Inställningar och välj **Lösningar**.

   ![](assets/eighteen.png)

1. Klicka på knappen **Publicera alla anpassningar**.

   ![](assets/nineteen.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

    * Om du vill begränsa antalet poster som du synkroniserar [konfigurera ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
    * Kör processen [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
    * Logga in i Marketo Sync User i Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Microsoft Dynamics med Marketo (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
