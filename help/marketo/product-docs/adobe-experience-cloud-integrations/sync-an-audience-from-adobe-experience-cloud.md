---
description: Synkronisera en målgrupp från Adobe Experience Cloud - Marketo Docs - Produktdokumentation
title: Synkronisera en publik från Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Synkronisera en publik från Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>En HIPAA-klar distribution av en Marketo-instans kan inte använda den här integreringen.

>[!PREREQUISITES]
>
>[Konfigurera organisationsmappning för Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Synkronisera en publik {#how-to-sync-an-audience}

1. I Min Marketo klickar du på **[!UICONTROL Database]** platta.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Klicka på **[!UICONTROL New]** nedrullningsbar meny och välj **[!UICONTROL Sync from Experience Cloud Audience]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Klicka på **[!UICONTROL Audience Library Folder]** och välj önskad ursprungsmapp.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Välj en **[!UICONTROL Audience Name]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. För målet kan du välja en befintlig lista eller skriva namnet på en ny. I det här exemplet skapar vi en ny. Klicka **[!UICONTROL Sync]** när det är klart.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Klicka på **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Vanliga frågor {#faq}

**Hur fungerar cookie-synkroniseringen?**

När cookie-synkronisering är aktiverat för din Marketo-prenumeration försöker Marketo munchkin.js hämta och lagra ECID:n för Adobe för den Adobe IMS-organisation som du angav under integreringsinställningen och matcha dessa ECID:n med motsvarande Marketo cookie-identifierare. Detta gör att Marketo anonyma användarprofiler kan berikas med ECID:n för Adobe.

Ytterligare ett steg krävs för att koppla den anonyma användarprofilen till en lead-profil, som identifieras med ett enkelt textmeddelande. Exakt hur det fungerar [beskrivs här](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Varför skiljer sig liststorleken i Marketo från den i Adobe?**

En person kan inte heller synkronisera över om vi inte kan koppla ett ECID-cookie-ID till en känd person i Marketo.

**Är detta en engångssynkronisering?**

Du behöver bara initiera synkroniseringen en gång. Därefter synkroniseras posterna automatiskt. Den inledande synkroniseringen kan ta upp till 24 timmar. nya poster kommer att synkas inom 2-3 timmar.
