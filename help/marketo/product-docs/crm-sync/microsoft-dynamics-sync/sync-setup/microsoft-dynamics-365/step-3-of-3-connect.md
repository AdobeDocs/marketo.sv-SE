---
unique-page-id: 3571830
description: Steg 3 av 3 - Anslut Microsoft Dynamics med Marketo (Online) - Marketo Docs - Produktdokumentation
title: Steg 3 av 3 -Anslut Microsoft Dynamics med Marketo (online)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Steg 3 av 3: Anslut Microsoft Dynamics med Marketo (Online) {#step-of-connect-microsoft-dynamics-with-marketo-online}

Detta är det sista steget i synkroniseringen. Vi är nästan framme!

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Installera Marketo-lösningen (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
   >
   >
* [Steg 2 av 3: Konfigurera Marketo Sync User i Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange Dynamics Sync-användarinformation {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **Admin**.

   ![](assets/login-admin.png)

1. Klicka på **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Välj **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Klicka på **Redigera** i **Steg 1: Ange autentiseringsuppgifter**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga inloggningsuppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **användarnamn**, **lösenord** och Microsoft Dynamics **URL** (klient-ID och klienthemlighet är valfria). Klicka på **Spara** när du är klar.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara user@domain.com eller DOMÄN\användare.

## Välj fält att synkronisera {#select-fields-to-sync}

1. Klicka på **Redigera** i **Steg 2: Välj Fält att synkronisera**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Markera de fält som du vill synkronisera med Marketo så att de är förmarkerade. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## Synkronisera fält för ett anpassat filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **Redigera** i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **Spara**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **Redigera** i **Steg 3: Aktivera synkronisering**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer eller leads manuellt.

1. Läs allt i popup-fönstret, ange din e-postadress och klicka på **Starta synkronisering**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Den första synkroniseringen kan ta några timmar. När det är klart får du ett e-postmeddelande.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Utmärkt arbete!
