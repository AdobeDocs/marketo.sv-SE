---
unique-page-id: 3571827
description: Steg 2 av 3 - Konfigurera Marketo Solution med Server to Server Connection - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Marketo Solution med Server to Server Connection
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Steg 2 av 3: Konfigurera Marketo Solution med Server to Server Connection {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo-lösningen med Server till server-anslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## Skapa klientprogram i [!DNL Azure AD] {#create-client-application-in-azure-ad}

1. Navigera till [den här Microsoft-artikeln](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Följ alla steg. I steg 3 anger du ett relevant programnamn (t.ex. [!DNL Marketo Integration]). Välj **Konto endast i den här organisationskatalogen** under de kontotyper som stöds.

1. Skriv ned program-ID (ClientId) och klient-ID. Du måste ange det i Marketo senare.

1. Ge administratörens samtycke genom att följa stegen [i den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Skapa en klienthemlighet i Admin Center genom att klicka på **[!UICONTROL Certificates & secrets]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Klicka på knappen **[!UICONTROL New client secret]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Ange en beskrivning av klienthemlighet och klicka på **[!UICONTROL Add]**.

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
   >* Observera programanvändarens e-postadress från alternativet [Visa information](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) på Power Platform. Den här e-postadressen används som användarnamn när anslutningen till MS [!DNL Dynamics] konfigureras i Marketo.

## [!DNL Azure AD] Federated med [!DNL AD FS On-prem] {#azure-ad-federated-with-ad-fs-on-prem}

För federerade [!DNL Azure AD] till [!DNL ADFS Onprem] måste en identifieringsprincip för hemsfär skapas för det specifika programmet. Med den här principen omdirigerar [!DNL Azure AD] autentiseringsbegäran till federationstjänsten. Synkronisering av lösenordshash måste aktiveras i [!DNL AD Connect] för detta. Mer information finns i [[!DNL OAuth] med [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) och [Ange en tredje princip för ett program](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Ytterligare referenser [finns här](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=Denna%20rapport%20innehåller även%20federerade%20är%20federerade%20till%20Azure%20AD.){target="_blank"}.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Allt vi har kvar är att informera Marketo Solution om den nya användaren som har skapats.

1. Gå tillbaka till avsnittet [!UICONTROL Advanced Settings], klicka på ikonen ![](assets/image2015-5-13-15-3a49-3a19.png) intill [!UICONTROL Settings] och välj **[!UICONTROL Marketo Config]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Uppdatera sidan om du inte ser &quot;Marketo Config&quot; på menyn Inställningar. Om det inte fungerar kan du försöka med att [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} igen eller logga ut och in igen.

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

   >[!NOTE]
   >
   >Om du uppgraderar från grundläggande autentisering till [!DNL OAuth] kan du använda [den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) för att konfigurera om din autentisering.

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar konfigurerar [ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Verifiera [!DNL Microsoft Dynamics] synkroniseringsprocessen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i [!DNL Microsoft Dynamics] CRM.

>[!MORELIKETHIS]
>
>* [Steg 3 av 3: Anslut Marketo-lösningen med Server till serveranslutning](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [Konfigurera om [!DNL Dynamics] autentiseringsmetod](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
