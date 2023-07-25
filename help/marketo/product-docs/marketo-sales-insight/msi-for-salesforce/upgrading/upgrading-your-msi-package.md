---
unique-page-id: 37357050
description: Uppgraderar ditt MSI-paket - Marketo Docs - produktdokumentation
title: Uppgraderar ditt MSI-paket
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Uppgraderar ditt MSI-paket {#upgrading-your-msi-package}

1. Navigera till [den här sidan i appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Logga in på din Salesforce-instans (den som är ansluten till din Marketo-instans, kan vara sandlåda eller produktion) från det övre högra hörnet på sidan från steg 1. Du måste ha administratörsbehörighet för att installera/uppgradera ett hanterat paket i Salesforce.

1. Klicka på **Hämta nu** -knappen. Du ombeds att välja var du vill installera. Du kan uppgradera eftersom du redan har en tidigare version av MSI. Välj ett alternativ baserat på det konto du loggade in på under steg 1.

   >[!TIP]
   >
   >Vi rekommenderar att du testar detta i din sandlådeinstans innan du uppgraderar din produktionsinstans.

1. Du kan uppgradera paketet genom att välja Installera endast för administratörer (och ge MSI-åtkomst till specifika profiler senare), Installera för alla användare eller Installera för specifika profiler. I det här exemplet väljer vi Endast administratörer. Klicka på **Uppgradera**.

   ![](assets/four.png)

>[!NOTE]
>
>Vi rekommenderar att du bara uppdaterar paketet för administratörer och sedan [ge åtkomst till specifika användare](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} baserat på antalet köpta MSI-licenser. Du kan också skapa en specifik Salesforce-profil för MSI-användare och installera eller uppgradera paketet endast för dessa användare.
