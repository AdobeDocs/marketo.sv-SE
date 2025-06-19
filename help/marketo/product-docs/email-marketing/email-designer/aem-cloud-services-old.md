---
title: Connect Experience Manager doc
description: Lär dig hur du ansluter Adobe Experience Manager Cloud Services till Adobe Marketo Engage så att du kan utnyttja dina AEM-resurser.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Anslut Adobe Experience Manager Cloud Services {#connect-adobe-experience-manager-cloud-services}

Lär dig hur du ansluter ditt AEM Assets Cloud Services-konto till din Adobe Marketo Engage-instans så att du kan utnyttja din AEM Asset-databas i Marketo Engage Email Designer.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **Admin** i Marketo Engage och välj **Adobe Experience Manager** i det vänstra navigeringsträdet.

SCREENSHOT

1. Klicka på **Redigera** bredvid _Adobe Experience Manager Cloud Services_.

SCREENSHOT

1. Markera en eller flera databaser.

SCREENSHOT

>[!NOTE]
>
>Endast databaser som har kopplats till samma IMS-organisation som din Marketo Engage-prenumeration visas.

1. Du måste lägga till ett [certifikat för tjänstautentiseringsuppgifter](https://experienceleague.adobe.com/sv/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) för att konfigurera databasen. Klicka på knappen **+ Lägg till certifikat**.

SCREENSHOT

1. Dra och släpp ditt certifikat (endast JSON-filen) eller välj det på datorn. Klicka på **Lägg till** när du är klar.

SCREENSHOT

1. Den konfigurerade databasen visas nedan tillsammans med status och utgångsdatum. Klicka på ellipsknappen (**..**) för att visa certifikatet. Annars är du klar.

SCREENSHOT

Nu kan du komma åt alla bilder från det digitala resurshanteringsbiblioteket i den databasen via Marketo Engage Email Designer.

>[!MORELIKETHIS]
>
>[Arbeta med Experience Manager-resurser](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
