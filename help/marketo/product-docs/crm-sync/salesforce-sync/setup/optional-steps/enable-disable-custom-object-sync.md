---
unique-page-id: 4719297
description: Aktivera/inaktivera anpassad objektsynkronisering - Marketo-dokument - Produktdokumentation
title: Aktivera/inaktivera synkronisering av anpassat objekt
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Aktivera/inaktivera synkronisering av anpassat objekt {#enable-disable-custom-object-sync}

Anpassade objekt som skapas i Salesforce-instansen kan också ingå i Marketo. Så här ställer du in det.

## Aktivera/inaktivera synkronisering av anpassat objekt {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Administratörsrättigheter krävs.

1. Klicka på **Admin**.

   ** ![](assets/one.png)

   **

1. Klicka på **Salesforce** **Objektsynkronisering** på menyn Databashantering.

   ![](assets/two-2.png)

1. Om det här är ditt första anpassade objekt klickar du på **Synkronisera schema.** Annars klickar du på  **Uppdatera** schema för att kontrollera att du har det senaste.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Om den globala synkroniseringen körs måste du inaktivera den genom att klicka på **Inaktivera global synkronisering.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Det kan ta några minuter att synkronisera det anpassade Salesforce-objektschemat.

1. Klicka på **Uppdatera schema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Markera det objekt som du vill synkronisera och klicka på **Aktivera synkronisering**.

   >[!TIP]
   >
   >Marketo kan bara synkronisera ett anpassat objekt om det har en direkt relation till lead-, kontakt- eller kontoobjektet i Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Klicka på **Aktivera synkronisering** igen.

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. Gå tillbaka till fliken **Salesforce** och klicka på **Aktivera synkronisering**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Använda dina anpassade objekt {#using-your-custom-objects}

>[!NOTE]
>
>Du kan inte använda anpassade objekt i smarta kampanjer med utlösare.

1. Dra över filtret **Har möjlighet** i den smarta listan och ställ in på&#x200B;**true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Använd sedan filterbegränsningar för att begränsa fokus.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Underbar! Nu kan du använda det här anpassade objektets data i smarta kampanjer och smarta listor.

>[!MORELIKETHIS]
>
>* [Lägg till/ta bort anpassat objektfält som smart lista/utlösarbegränsningar](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>



