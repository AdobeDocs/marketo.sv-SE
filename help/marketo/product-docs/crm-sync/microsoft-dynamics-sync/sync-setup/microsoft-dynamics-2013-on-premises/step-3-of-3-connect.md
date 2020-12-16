---
unique-page-id: 3571819
description: Steg 3 av 3 - Connect Marketo och Dynamics (2013 On-Premises) - Marketo Docs - Produktdokumentation
title: Steg 3 av 3 - Connect Marketo och Dynamics (2013 On-Premises)
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---


# Steg 3 av 3: Connect Marketo och Dynamics (On-Premises 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

Okej! Vi installerade lösningen och konfigurerade synkroniseringsanvändaren. Därefter måste vi koppla Marketo och Dynamics.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Installera Marketo-lösningen i Dynamics (On-Premises 2013)](step-1-of-3-install.md)
>* [Steg 2 av 3: Konfigurera Synkronisera användare för Marketo (lokal 2013)](step-2-of-3-configure.md)

>



>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange användarinformation för Dynamics Sync {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **Admin**.

   ![](assets/login-admin.png)

1. Klicka på **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Välj **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicka på **REDIGERA** i **steg 1: Ange autentiseringsuppgifter**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga inloggningsuppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **användarnamn**, **lösenord** och Microsoft Dynamics- **URL** och klicka sedan på **SPARA**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#631610061123070c0e020a0d4d000c0e) DOMAIN\user.

   >[!TIP]
   >
   >Vet du inte URL:en? Vi visar hur du hittar URL:en [till](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics-organisationstjänsten här.

## Markera fält som ska synkroniseras {#select-fields-to-sync}

Nu måste vi markera de fält vi vill synkronisera.

1. Klicka på **REDIGERA **i **steg 2: Markera de fält som ska synkroniseras**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Markera de fält som du vill synkronisera med Marketo så att de är förmarkerade. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## Synkronisera fält för ett eget filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **Redigera** i fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **REDIGERA **i **steg 3: Aktivera synkronisering**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer eller leads manuellt.

1. Läs allt i popup-fönstret, ange ditt e-postmeddelande och klicka på **START SYNC**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Den första synkroniseringen kan ta några timmar. När det är klart får du ett e-postmeddelande.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Utmärkt arbete! Du har just frigjort kraften i den dubbelriktade synkroniseringen mellan Marketo och Microsoft Dynamics. Om du har köpt Marketo Sales Insight är det roligare att få:

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013](../../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)

>



