---
unique-page-id: 9438139
description: Lägg till person i Blockeringslista - Marketo Docs - produktdokumentation
title: Lägg till person i Blockeringslista
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Lägg till person i Blockeringslista {#add-person-to-blocklist}

Genom att lägga till personer på Blockeringslista kan de inte ta emot din korrespondens.

>[!NOTE]
>
>Marketo håller på att ändra termer som Blacklist och Whitelist för att Blocklist och Tillåtslista i vår produkt. Under den här uppdateringen kan du se de gamla villkoren i våra användargränssnitt och skärmbilder för dokumentation samt de nya villkoren i vår dokumentationstext. Vi ber om ursäkt för all förvirring.

1. [Skapa ett nytt standardprogram](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) och namnge **Lägg till i Blockeringslista**.

1. Klicka **Nytt** och markera **Ny lokal resurs**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Namnge listan och klicka på **Skapa**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Lägg till alla personer i **Smart List** som du vill lägga till i Blockeringslista.

   >[!NOTE]
   >
   >Personer på ditt Blockeringslista får inte några operativa e-postmeddelanden.

   ![](assets/three-6.png)

1. Klicka **Nytt** och markera **Ny smart kampanj**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Namnge **Ny smart kampanj**. Klicka **Skapa**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Dra och släpp **Medlem i Smart List**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Välj den smarta listan som du nyss skapade.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Dra och släpp **Ändra datavärde**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. För **Flöde**, ange **Blocklista** för **Attribut** och ange **Nytt värde** till **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. På **Schema** flik, välja **Kör en gång**.

   ![](assets/ten.png)

1. Välj **Kör nu** och klicka **Kör**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   YAY! Dessa personer kommer inte längre att få e-post.

   >[!TIP]
   >
   >Skapa en [utlösa smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) använda **Ändra datavärde** med **Blocklistan är sann** för alla i framtiden som har attribut som kan blocklist.
