---
description: Steg 2 av 3 - Konfigurera Marketo Solution med Resource Owner Password Control Connection - Marketo Docs - Product Documentation
title: Steg 2 av 3 - Konfigurera Marketo Solution med Resource Owner Password Control Connection
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Steg 2 av 3: Konfigurera Marketo Solution med Resource Owner Password Control Connection {#step-2-of-3-set-up-the-marketo-solution-ropc}

Vi börjar med att skapa ett användarkonto.

>[!PREREQUISITES]
>
>[Steg 1 av 4: Installera Marketo Solution med Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## Skapa en ny användare {#create-a-new-user}

1. Logga in i Dynamics. Klicka på ikonen Inställningar och välj **Avancerade inställningar**.

   ![](assets/one.png)

1. Klicka **Inställningar** och markera **Säkerhet**.

   ![](assets/two.png)

1. Klicka **Användare**.

   ![](assets/three.png)

1. Klicka **Nytt.**

   ![](assets/four.png)

1. Klicka **Lägg till och licensiera användare** i det nya fönstret.

   ![](assets/five.png)

1. En ny flik öppnas. Klicka **Administratör** överst på sidan.

   ![](assets/six.png)

1. En annan ny flik öppnas. Klicka **Lägg till en användare**.

   ![](assets/seven.png)

1. Ange all information. När du är klar klickar du på **Lägg till**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Det här namnet måste vara en dedikerad synkroniseringsanvändare och inte en befintlig CRM-användares konto. Det behöver inte vara en faktisk e-postadress.

1. Ange e-postadressen som ska ta emot inloggningsuppgifterna och klicka på **Skicka e-post och stäng**.

   ![](assets/nine.png)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Om du vill uppgradera Marketo går du till [Uppgradera Marketo Solution för Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Språkinställningen för Synkronisera användare [ska anges till engelska](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Gå tillbaka till fliken Aktiverade användare och uppdatera användarlistan.

   ![](assets/ten.png)

1. Hovra bredvid den nya Marketo Sync-användaren så visas en kryssruta. Klicka för att markera den.

   ![](assets/eleven.png)

1. Klicka **Hantera roller**.

   ![](assets/twelve.png)

1. Kontrollera **Marketo Sync User** och klicka **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare kommer att **not** synkas tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Allt vi har kvar är att informera Marketo Solution om den nya användaren som har skapats.

1. Gå tillbaka till avsnittet Avancerade inställningar och klicka på ![](assets/image2015-5-13-15-3a49-3a19.png) -ikon bredvid Inställningar och välj **Marketo Config**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Om du inte ser **Marketo Config** Uppdatera sidan på menyn Inställningar. Om det inte fungerar, försök [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) igen eller logga ut och in igen.

1. Klicka **Standard**.

   ![](assets/fifteen.png)

1. Klicka på sökknappen på **Marketo-användare** och välj den synkroniseringsanvändare du skapade.

   ![](assets/sixteen.png)

1. Klicka på ![](assets/image2015-3-13-15-3a10-3a11.png) i det nedre högra hörnet om du vill spara ändringarna.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicka på **X** i det övre högra hörnet för att stänga skärmen.

   ![](assets/seventeen.png)

1. Klicka på ![](assets/image2015-5-13-15-3a49-3a19-1.png) -ikon bredvid Inställningar och välj **Lösningar**.

   ![](assets/eighteen.png)

1. Klicka på **Publicera alla anpassningar** -knappen.

   ![](assets/nineteen.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar, [konfigurera ett eget synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) -processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in i Marketo Sync User i Microsoft Dynamics CRM.

   >[!MORELIKETHIS]
   >
   >[Steg 3 av 4: Anslut Marketo Solution med Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
