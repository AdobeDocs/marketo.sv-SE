---
description: Konfigurera Microsoft Dynamics CRM-appen för On-prem - Marketo Docs - Produktdokumentation
title: Konfigurera Microsoft Dynamics CRM-appen för lokal installation
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Konfigurera Microsoft Dynamics CRM-appen för lokal {#set-up-microsoft-dynamics-crm-app-for-on-prem}

Klient-ID/klienthemlighetsbaserad konfiguration i Marketo kan göras för lokal anslutning med AD FS (ver). 2016 eller senare). För äldre versioner av On-prem ber vi dig kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) för att få autentiseringsmetoden ändrad så att den bara baseras på användar-ID och lösenord.

## Konfigurera Microsoft Dynamics CRM-appen {#set-up-microsoft-dynamics-crm-app}

Följ stegen i [den här Microsoft-artikeln](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later).

När du är klar är nästa steg att **ange det Dynamics CRM-genererade klient-ID:t och hemligheten i Marketo**.

## Ange det Dynamics CRM-genererade klient-ID:t och hemligheten i Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

Följande steg gäller för online- och On-prem-versioner.

1. I Marketo klickar du på **Admin**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. Klicka på **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. Klicka på **Inaktivera synkronisering**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. Klicka på **Redigera** bredvid autentiseringsuppgifter.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. Ange **klient-ID** och **Klienthemlighet** som du hämtade tidigare och tryck på **Spara**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. Klicka på **Verifiera synkroniseringsinställningar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. Klicka på **Nästa**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. Alla gröna bockar ska visas. Klicka på **Stäng**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >Om du ser ett rött X bland de gröna bockmarkeringarna läser du [den här artikeln](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) för korrigeringsalternativ.

1. Klicka på **Aktivera synkronisering**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

Och det är allt!
