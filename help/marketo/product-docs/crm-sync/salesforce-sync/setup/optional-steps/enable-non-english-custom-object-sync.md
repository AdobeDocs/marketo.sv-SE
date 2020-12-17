---
unique-page-id: 4719302
description: Aktivera icke-engelsk anpassad objektsynkronisering - Marketo Docs - produktdokumentation
title: Aktivera icke-engelsk anpassad objektsynkronisering
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Aktivera icke-engelsk anpassad objektsynkronisering {#enable-non-english-custom-object-sync}

Om Marketo-synkroniseringsanvändaren är inställd på ett annat språk än engelska kan du råka ut för ett fel när du försöker aktivera en anpassad objektsynkronisering.

## Felet {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Komma runt det {#getting-around-it}

1. Logga in i Salesforce med markeringen för att synkronisera användaren.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Gå till **Inställningar** under användarnamnet.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Under **Personlig information** klickar du på **Min personliga information**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicka på **Redigera**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändra **Språk** till **Engelska**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicka på **Spara**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Tillbaka till Marketo, under **Admin > Salesforce > Objekt** klickar du på **Uppdatera schema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Objektivlistan kommer då att visas på engelska. Markera det objekt du vill använda och klicka på **Aktivera synkronisering**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observera att ditt anpassade objekt nu är aktiverat och synkroniseras.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Gå nu tillbaka till Salesforce och använd stegen ovan för att ändra synkroniseringsanvändaren tillbaka till det språk du föredrar.

>[!NOTE]
>
>**Påminnelse**
>
>Glöm inte att uppdatera schemat en sista gång för att hämta tillbaka objekten på ditt språk.

