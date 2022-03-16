---
unique-page-id: 3571830
description: Steg 3 av 3 - Ansluta Marketo-lösningen med Server to Server Connection - Marketo Docs - Produktdokumentation
title: Steg 3 av 3 - Ansluta Marketo Solution med Server to Server Connection
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
source-git-commit: 5536b35d71506f11fdf32bf7149bf5c61174ab34
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Steg 3 av 3: Ansluta Marketo-lösningen med server-till-server-anslutning {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

Detta är det sista steget i synkroniseringen. Vi är nästan framme!

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Installera Marketo Solution with Server to Server Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [Steg 2 av 3: Konfigurera Marketo Solution med Server to Server Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!IMPORTANT]
>
>Om du uppgraderar från grundläggande autentisering till OAuth måste du kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support) om du vill ha hjälp med att uppdatera ytterligare parametrar. Om du aktiverar den här funktionen avbryts synkroniseringen tillfälligt tills nya autentiseringsuppgifter anges och synkroniseringen aktiveras igen. Funktionen kan inaktiveras (fram till april 2022) om du vill återgå till det gamla autentiseringsläget.

>[!NOTE]
>
>Innan du anger nya autentiseringsuppgifter kan du [validera dem här](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

## Ange användarinformation för Dynamics Sync {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka **Administratör**.

   ![](assets/login-admin.png)

1. Klicka på **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Välj **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Klicka **Redigera** in **Steg 1: Ange autentiseringsuppgifter**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Kontrollera att din organisations-URL är korrekt eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om en felaktig Org URL används måste du skaffa en ny Marketo-prenumeration. Om du inte känner till URL:en [lära dig hur du hittar det här](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. Ange användarinformationen för Dynamics Sync och klicka på **Spara** när det är klart.

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Användarnamnet i Marketo måste matcha [e-postadress](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) för programanvändaren i CRM. Formatet kan vara `user@domain.com` eller DOMÄN\användare.

## Markera fält som ska synkroniseras {#select-fields-to-sync}

1. Klicka **Redigera** in **Steg 2: Markera fält som ska synkroniseras**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Markera de fält som du vill synkronisera till Marketo så att de är förmarkerade. Klicka **Spara**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo lagrar en referens till de fält som ska synkroniseras. Om du tar bort ett fält i Dynamics rekommenderar vi att du gör det med [synkronisering inaktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Uppdatera sedan schemat i Marketo genom att redigera och spara [Markera fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Synkronisera fält för ett eget filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka **Redigera** i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka **Spara**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka **Redigera** in **Steg 3: Aktivera synkronisering**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer eller leads manuellt.

1. Läs allt i popup-fönstret, ange din e-postadress och klicka på **Starta synkronisering**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Den första synkroniseringen kan ta några timmar. När det är klart får du ett e-postmeddelande.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Utmärkt arbete!
