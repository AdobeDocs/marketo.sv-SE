---
title: Connect Experience Manager doc
description: Lär dig hur du kopplar Adobe Experience Manager-Cloud Service till Adobe Marketo Engage så att du kan utnyttja dina AEM resurser.
source-git-commit: 92404e10771920862cd147c09e2ada37484e6118
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Anslut Adobe Experience Manager-Cloud Service {#connect-adobe-experience-manager-cloud-services}

Lär dig hur du ansluter ditt AEM Assets Cloud Services-konto till din Adobe Marketo Engage-instans så att du kan utnyttja ditt AEM i Marketo Engage e-postkonto i Designer.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **Admin** i Marketo Engage och välj **Adobe Experience Manager** i det vänstra navigeringsträdet.

   ![Välj Adobe Experience Manager i administratörsavsnittet](assets/connect-adobe-experience-manager-cloud-services-1.png){width="800"}

1. Klicka på **Redigera** bredvid _Adobe Experience Manager-Cloud Service_.

   ![Klicka på REDIGERA](assets/connect-adobe-experience-manager-cloud-services-2.png){width="400"}

1. Markera en eller flera databaser.

   ![Välj en databas](assets/connect-adobe-experience-manager-cloud-services-3.png){width="800"}

   >[!NOTE]
   >
   >Endast databaser som har kopplats till samma IMS-organisation som din Marketo Engage-prenumeration visas.

1. Du måste lägga till ett [certifikat för tjänstautentiseringsuppgifter](https://experienceleague.adobe.com/sv/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) för att konfigurera databasen. Klicka på knappen **+ Lägg till certifikat**.

   ![Lägg till ett certifikat](assets/connect-adobe-experience-manager-cloud-services-4.png){width="800"}

1. Dra och släpp ditt certifikat (endast JSON-filen) eller välj det på datorn. Klicka på **Lägg till** när du är klar.

   ![Leta reda på certifikatet på datorn](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

1. Den konfigurerade databasen visas nedan tillsammans med status och utgångsdatum. Klicka på ellipsknappen (**..**) för att visa certifikatet. Annars är du klar.

   ![Certifikatet har lagts till](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

Nu kan du nå alla bilder från det digitala resurshanteringsbiblioteket i den databasen via Marketo Engage Email Designer.

>[!MORELIKETHIS]
>
>[Arbeta med Experience Manager-resurser](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
