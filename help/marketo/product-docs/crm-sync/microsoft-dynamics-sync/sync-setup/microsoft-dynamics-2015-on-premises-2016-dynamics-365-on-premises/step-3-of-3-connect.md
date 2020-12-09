---
unique-page-id: 7504744
description: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 3 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 3 of 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 3 of 3 {#install-marketo-for-dynamics-on-prem-and-on-prem-step-of}

>[!PREREQUISITES]
>
>* [Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 1 of 3](step-1-of-3-install.md)
>* [Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 2 of 3](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange användarinformation för Dynamics Sync {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **Admin**.

   ![](assets/login-admin.png)

1. Klicka på **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Välj **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicka på **Redigera** i **steg 1: Ange autentiseringsuppgifter**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga inloggningsuppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **användarnamn**, **lösenord** för en Microsoft Dynamics- **URL** och ett valfritt **klient-ID**. Klicka på **Spara** när du är klar.

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#8cf9ffe9fecce8e3e1ede5e2a2efe3e1) DOMAIN\user.

   >[!TIP]
   >
   >Vet du inte URL:en? Här visas hur du hittar URL:en [till](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics-organisationstjänsten.

## Markera fält som ska synkroniseras {#select-fields-to-sync}

1. Klicka på **Redigera** i **steg 2: Markera de fält som ska synkroniseras**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Markera de fält som du vill synkronisera med Marketo så att de är förmarkerade. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Synkronisera fält för ett eget filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **Redigera** i fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **Redigera** i **steg 3: Aktivera synkronisering**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer manuellt.

1. Läs allt i popup-fönstret, ange ditt e-postmeddelande och klicka på **Starta synkronisering**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Den första synkroniseringen kan ta några timmar. När det är klart får du ett e-postmeddelande.

   ![](assets/image2015-3-16-9-59-51.png)

Utmärkt arbete!
