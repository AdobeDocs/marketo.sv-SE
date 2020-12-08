---
unique-page-id: 3571809
description: Steg 3 av 3 - Ansluta Microsoft Dynamics med Marketo (2011 On-Premises) - Marketo Docs - Produktdokumentation
title: Steg 3 av 3 - Anslut Microsoft Dynamics med Marketo (On-Premises 2011)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# Steg 3 av 3: Anslut Microsoft Dynamics med Marketo (On-Premises 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Okej! Vi installerade lösningen och konfigurerade synkroniseringsanvändaren. Därefter måste vi koppla Marketo och Dynamics.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Installera Marketo-lösningen (2011 On-Premises)](step-1-of-3-install.md)
>* [Steg 2 av 3: Konfigurera Marketo-synkronisering av användare i Dynamics (lokal 2011)](step-2-of-3-set-up.md)


>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange användarinformation för Dynamics Sync {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **Admin**.

   ![](assets/login-admin.png)

1. Klicka på **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Klicka på **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicka på **Redigera** i **steg 1: Ange autentiseringsuppgifter.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga inloggningsuppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **användarnamn**, **lösenord** och CRM- **URL** och klicka sedan på **Spara**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) DOMAIN\user.

   >[!TIP]
   >
   >Vet du inte URL:en? Vi visar hur du hittar URL:en [till](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics-organisationstjänsten här.

## Markera fält som ska synkroniseras {#select-fields-to-sync}

Nu måste vi markera de fält vi vill synkronisera.

1. Klicka på **Redigera** i **steg 2: Markera de fält som ska synkroniseras.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Det finns förmarkerade fält som kommer att synkroniseras. Lägg till mer om du vill och klicka på **Spara**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## Synkronisera fält för ett eget filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **Redigera** i fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **Spara**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **Redigera** i **steg 3: Aktivera synkronisering**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer eller leads manuellt.

1. Läs allt i popup-fönstret, ange ditt e-postmeddelande och klicka på **Starta synkronisering**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Den första synkroniseringen kan ta några timmar. När det är klart får du ett e-postmeddelande.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Utmärkt arbete!
