---
description: Steg 3 av 4 - Konfigurera klientapp för MS Dynamics - Marketo Docs - Produktdokumentation
title: Steg 3 av 4 - Konfigurera klientappen för MS Dynamics
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Steg 3 av 4: Konfigurera klientapp för MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Steg 1 av 4: Installera Marketo Solution med Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Steg 2 av 4: Konfigurera Marketo Solution med Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Navigera till detta [Microsoft-artikel](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Följ alla steg. I steg 3 anger du ett relevant programnamn (t.ex.&quot;Marketo Integration&quot;). Välj Konto endast i den här organisationskatalogen under Kontotyper som stöds.

1. Skriv ned program-ID (ClientId). Du måste ange det i Marketo senare.

1. Ge administratörens samtycke genom att följa stegen i [den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Generera en klienthemlighet i Admin Center genom att klicka på **[!UICONTROL Certificates & secrets]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Klicka på **[!UICONTROL New client secret]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Lägg till en beskrivning av klienthemlighet och klicka på **[!UICONTROL Add]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Observera värdet för Klienthemlighet (visas i skärmbilden nedan), som du behöver det senare. Den visas bara en gång och du kommer inte att kunna hämta den igen.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated med AD FS On-prem {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD till ADFS OnPrem måste skapa en identifieringsprincip för hemsfär för det specifika programmet. Med den här principen dirigerar Azure AD om autentiseringsbegäran till federationstjänsten. Synkronisering av lösenordshash måste aktiveras i AD Connect för detta. Mer information finns på [OAuth med ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Ytterligare referenser [finns här](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=Denna%20rapport%20innehåller även%20federerade%20är%20federerade%20till%20Azure%20AD.){target="_blank"}.

## Innan du fortsätter till steg 4 {#before-proceeding-to-step-4}

* Om du vill begränsa antalet poster som du synkroniserar, [konfigurera ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} nu.
* Kör [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} -processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Steg 4 av 4: Anslut Marketo Solution med Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
