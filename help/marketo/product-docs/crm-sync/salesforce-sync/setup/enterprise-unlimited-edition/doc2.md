---
description: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Dessa steg måste utföras av en Salesforce-administratör

>[!PREREQUISITES]
>
>[Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

I den här artikeln ska du ange användarbehörigheter i Salesforce-profilen och skapa ett Marketo-Salesforce-integrationskonto.

## Skapa en profil {#create-a-profile}

1. Klicka på **[!UICONTROL Setup]**.

   SCREENSHOT

1. Skriv &quot;profiler&quot; i navigeringsfältet och klicka på länken Profiler.

   SCREENSHOT

1. Klicka på Ny profil.

   SCREENSHOT

1. Välj Standardanvändare, ge profilen namnet&quot;Marketo-Salesforce Sync&quot; och klicka på Spara.

   SCREENSHOT

## Ange profilbehörigheter {#set-profile-permissions}

1. Klicka på Redigera för att ange säkerhetsbehörigheter.

   SCREENSHOT

1. Kontrollera att följande rutor är markerade under Administrativa behörigheter:

   * API aktiverat
   * Redigera HTML-mallar
   * Hantera offentliga dokument
   * Hantera offentliga mallar

   >[!TIP]
   >
   >Markera rutan Lösenordet upphör aldrig att gälla.

1. Kontrollera att följande rutor är markerade under avsnittet Allmänna användarbehörigheter:

   * Konvertera leads
   * Redigera händelser
   * Redigera uppgifter

1. Under avsnittet Standardbehörigheter för objekt kontrollerar du att behörigheterna Läs, Skapa, Redigera och Ta bort är ikryssade:

   * Konton
   * Kampanjer
   * Kontakter
   * Leads
   * Möjligheter

   >[!NOTE]
   >
   >Bevilja behörigheter till kampanjerna om du tänker använda kampanjsynkronisering.

   SCREENSHOT

1. När du är klar klickar du på Spara längst ned på sidan.

   SCREENSHOT

## Ange fältbehörigheter {#set-field-permissions}

1. Diskutera med era marknadsförare för att ta reda på vilka anpassade fält som behövs för att synkronisera.

   >[!NOTE]
   >
   >Det här steget förhindrar att fält som du inte behöver visas i Marketo, vilket gör att det blir rörigt och snabbar upp synkroniseringen.

1. Gå till avsnittet Fältnivåsäkerhet på profilinformationssidan. Klicka på Visa för att redigera tillgängligheten för objekten:

   * Lead
   * Kontakt
   * Konto
   * Möjligheter

   >[!TIP]
   >
   >Du kan konfigurera andra objekt efter organisationens behov.

1. Klicka på Redigera för varje objekt.

   SCREENSHOT

1. Leta reda på de fält som inte behövs, kontrollera att Läs åtkomst och Redigera åtkomst är avmarkerade. Klicka på Spara när du är klar.

   >[!NOTE]
   >
   >Redigera bara tillgängligheten för anpassade fält.

   SCREENSHOT

1. När du har avaktiverat alla onödiga fält måste du kontrollera Läs åtkomst och Redigera åtkomst för följande objektfält. Klicka på Spara när du är klar.

   TABELL

   SCREENSHOT

## Skapa Marketo-Salesforce Sync-konto {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Skapa ett dedikerat Salesforce-konto (t.ex. `marketo@yourcompany.com`) för att skilja mellan Marketo och andra Salesforce-användare.

1. Skriv&quot;Hantera användare&quot; i navigeringsfältet och klicka sedan på Användare. Klicka på Ny användare.

   SCREENSHOT

   SCREENSHOT

1. Fyll i obligatoriska fält. Välj sedan användarlicens: Salesforce och den profil som du skapade tidigare. Klicka på Spara när du är klar.

   SCREENSHOT

Steg 2 av 3 är slutförd.
