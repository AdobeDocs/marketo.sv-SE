---
unique-page-id: 7504744
description: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 3 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 3 of 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Steg 3 av 3: Connect Marketo Dynamics (2015 On-Prem och 2016 365 On-Prem) {#step-of-connect-marketo-dynamics-on-premises-and-365}

>[!PREREQUISITES]
>
>* [Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 1 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 2 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange Dynamics Sync-användarinformation {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **Admin**.

   ![](assets/login-admin.png)

1. Klicka på **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Välj **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicka på **Redigera** i **Steg 1: Ange autentiseringsuppgifter**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga inloggningsuppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **användarnamn**, **lösenord** en Microsoft Dynamics **URL** och ett valfritt **klient-ID**. Klicka på **Spara** när du är klar.

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara user@domain.com eller DOMÄN\användare.

   >[!TIP]
   >
   >Vet du inte URL:en? Vi visar dig hur du hittar din [Dynamics organisationstjänst-URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) här.

## Välj fält att synkronisera {#select-fields-to-sync}

1. Klicka på **Redigera** i **Steg 2: Välj Fält att synkronisera**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Markera de fält som du vill synkronisera med Marketo så att de är förmarkerade. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Synkronisera fält för ett anpassat filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **Redigera** i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **Redigera** i **Steg 3: Aktivera synkronisering**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer manuellt.

1. Läs allt i popup-fönstret, ange ditt e-postmeddelande och klicka på **Starta synkronisering**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Den första synkroniseringen kan ta några timmar. När det är klart får du ett e-postmeddelande.

   ![](assets/image2015-3-16-9-59-51.png)

Utmärkt arbete!
