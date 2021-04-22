---
description: Konfigurera MSD för Azure AD Federated med AD FS On-prem, Tenant och Microsoft Online - Marketo Docs - produktdokumentation
title: Konfigurera MSD för Azure AD Federated med AD FS On-prem, Tenant och Microsoft Online
exl-id: b6c10048-d27e-4135-beef-232deddc2984
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Konfigurera MSD för Azure AD Federated med AD FS On-prem, Tenant och Microsoft Online {#set-up-msd-for-azure-ad-federated-with-ad-fs-on-prem-tenant-and-microsoft-online}

## Konfigurera Microsoft Dynamics CRM-appen {#set-up-microsoft-dynamics-crm-app}

1. Gå till https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Följ alla steg. I steg 3 anger du ett relevant programnamn (t.ex.&quot;Marketo Integration&quot;). Välj Konto endast i den här organisationskatalogen under Kontotyper som stöds.

1. Skriv ned program-ID (ClientId). Du måste ange det i Marketo senare.

1. Ge administratörens samtycke genom att följa stegen i [den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md).

1. Skapa en klienthemlighet i Admin Center genom att klicka på **Certifikat och hemligheter**.

   ![](assets/set-up-msd-for-azure-ad-federated-1.png)

1. Klicka på **Ny klienthemlighet**.

   ![](assets/set-up-msd-for-azure-ad-federated-2.png)

1. Lägg till en beskrivning av klienthemlighet och klicka på **Lägg till**.

   ![](assets/set-up-msd-for-azure-ad-federated-3.png)

   >[!CAUTION]
   >
   >Observera värdet för Klienthemlighet (visas i skärmbilden nedan), som du behöver det senare. Den visas bara en gång och du kommer inte att kunna hämta den igen.

   ![](assets/set-up-msd-for-azure-ad-federated-4.png)

Marketo autentiserar till Azure AD med OAuth med hjälp av grant_type Resource Owner Password Credentials( ROPC). I det här scenariot måste en hemsökningsprincip skapas för det specifika programmet. Med den här principen dirigerar Azure AD om autentiseringsbegäran till federationstjänsten. Synkronisering av lösenordshash måste aktiveras i AD Connect för detta. Mer information finns i [OAuth med ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) och [Ange en extern princip för ett program](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Ytterligare referenser [finns här](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=Denna%20rapport%20innehåller även%20federerade%20är%20federerade%20till%20Azure%20AD.).

När du är klar är det dags att **ange det Dynamics CRM-genererade klient-ID:t och hemligheten i Marketo**.

## Ange det Dynamics CRM-genererade klient-ID och hemlighet i Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

1. Klicka på **Admin** i Marketo.

   ![](assets/set-up-msd-for-azure-ad-federated-5.png)

1. Klicka på **Microsoft Dynamics**.

   ![](assets/set-up-msd-for-azure-ad-federated-6.png)

1. Klicka på **Inaktivera synkronisering**.

   ![](assets/set-up-msd-for-azure-ad-federated-7.png)

1. Klicka på **Redigera** bredvid autentiseringsuppgifter.

   ![](assets/set-up-msd-for-azure-ad-federated-8.png)

1. Ange **klient-ID** och **Klienthemlighet** som du hämtade tidigare och tryck på **Spara**.

   ![](assets/set-up-msd-for-azure-ad-federated-9.png)

1. Klicka på **Verifiera synkroniseringsinställningar**.

   ![](assets/set-up-msd-for-azure-ad-federated-10.png)

1. Klicka på **Nästa**.

   ![](assets/set-up-msd-for-azure-ad-federated-11.png)

1. Alla gröna bockar ska visas. Klicka på **Stäng**.

   ![](assets/set-up-msd-for-azure-ad-federated-12.png)

   >[!NOTE]
   >
   >Om du ser ett rött X bland de gröna bockmarkeringarna läser du [den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) för korrigeringsalternativ.

1. Klicka på **Aktivera synkronisering**.

   ![](assets/set-up-msd-for-azure-ad-federated-13.png)

Och det är allt!
