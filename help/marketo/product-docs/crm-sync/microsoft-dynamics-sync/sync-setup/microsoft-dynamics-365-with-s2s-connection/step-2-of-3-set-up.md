---
unique-page-id: 3571827
description: Steg 2 av 3 - Konfigurera Marketo Solution med Server to Server Connection - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Marketo Solution med Server to Server Connection
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# Steg 2 av 3: Konfigurera Marketo Solution med Server to Server Connection {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo Solution with Server to Server Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## Skapa klientprogram i Azure AD {#create-client-application-in-azure-ad}

1. Navigera till [den här Microsoft-artikeln](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Följ alla steg. I steg 3 anger du ett relevant programnamn (t.ex.&quot;Marketo Integration&quot;). Under de kontotyper som stöds väljer du **Konto endast i den här organisationskatalogen**.

1. Skriv ned program-ID (ClientId) och klient-ID. Du måste ange det i Marketo senare.

1. Ge administratörens samtycke genom att följa stegen [i den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Generera en klienthemlighet i Admin Center genom att klicka på **Certifikat och hemligheter**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Klicka på **Ny klienthemlighet** -knappen.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Ange en beskrivning av klienthemligheten och klicka på **Lägg till**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>Observera värdet för Klienthemlighet (visas i skärmbilden nedan), som du behöver det senare. Den visas bara en gång och du kommer inte att kunna hämta den igen.

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Skapa programanvändare i Microsoft {#create-application-user-in-microsoft}

1. Följ stegen från följande länk för att [konfigurera en programanvändare i Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* När du ger behörighet till programanvändaren måste du tilldela den till&quot;Marketo Sync User Role&quot;.
   >* Anteckna programmets användares e-postadress från [visningsalternativ](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} på Power Platform. Den här e-postadressen används som användarnamn när du konfigurerar anslutningen till MS Dynamics i Marketo.
   >* Alla uppdateringar som görs i CRM av Synkronisera användare kommer att **not** synkas tillbaka till Marketo.

## Azure AD Federated med AD FS On-prem {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD till ADFS OnPrem måste skapa en identifieringsprincip för hemsfär för det specifika programmet. Med den här principen dirigerar Azure AD om autentiseringsbegäran till federationstjänsten. Synkronisering av lösenordshash måste aktiveras i AD Connect för detta. Mer information finns på [OAuth med ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Ytterligare referenser [finns här](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=Denna%20rapport%20innehåller även%20federerade%20är%20federerade%20till%20Azure%20AD.){target="_blank"}.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Allt vi har kvar är att informera Marketo Solution om den nya användaren som har skapats.

1. Gå tillbaka till avsnittet Avancerade inställningar och klicka på ![](assets/image2015-5-13-15-3a49-3a19.png) -ikon bredvid Inställningar och välj **Marketo Config**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Om du inte ser **Marketo Config** Uppdatera sidan på menyn Inställningar. Om det inte fungerar, försök [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} igen eller logga ut och in igen.

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

   >[!NOTE]
   >
   >Om du uppgraderar från grundläggande autentisering till OAuth kan du använda [den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} för att konfigurera om din autentisering.

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar, [konfigurera ett eget synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} nu.
* Kör [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} -processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Steg 3 av 3: Ansluta Marketo-lösningen med server-till-server-anslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md){target="_blank"}
>* [Konfigurera om Dynamics-autentiseringsmetod](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
