---
unique-page-id: 4719302
description: Aktivera icke-engelsk anpassad objektsynkronisering - Marketo Docs - produktdokumentation
title: Aktivera icke-engelsk anpassad objektsynkronisering
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 1%

---

# Aktivera icke-engelsk anpassad objektsynkronisering {#enable-non-english-custom-object-sync}

Om din Marketo-synkroniseringsanvändare är inställd på ett annat språk än engelska kan du råka ut för ett fel när du försöker aktivera en anpassad objektsynkronisering.

## Felet {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Komma runt {#getting-around-it}

1. Logga in på [!DNL Salesforce] med markeringen för att synkronisera användaren.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Gå till **[!UICONTROL Setup]** under användarnamnet.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Klicka på **[!UICONTROL Personal Information]** under **[!UICONTROL My Personal Information]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändra **[!UICONTROL Language]** till **[!UICONTROL English]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. I Marketo, under **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objects]**, klickar du på **[!UICONTROL Refresh Schema]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Objektivlistan kommer då att visas på engelska. Välj det objekt du vill använda och klicka sedan på **[!UICONTROL Enable Sync]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observera att ditt anpassade objekt nu är aktiverat och synkroniseras.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Gå tillbaka till [!DNL Salesforce] och använd stegen ovan för att ändra synkroniseringsanvändaren tillbaka till det språk du föredrar.

>[!NOTE]
>
>Glöm inte att uppdatera schemat en sista gång för att hämta tillbaka objekten på ditt språk.
