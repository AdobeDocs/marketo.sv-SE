---
unique-page-id: 9438139
description: Lägg till person i Blockeringslista - Marketo Docs - Produktdokumentation
title: Lägg till person i Blockeringslista
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Lägg till person i Blockeringslista {#add-person-to-blocklist}

Genom att lägga till personer på Blockeringslista kan de inte ta emot din korrespondens.

>[!NOTE]
>
>Marketo håller på att ändra termer som Blacklist och Whitelist för att Blocklist och Tillåtslista i vår produkt. Under den här uppdateringen kan du se de gamla villkoren i våra användargränssnitt och skärmbilder för dokumentation samt de nya villkoren i vår dokumentationstext. Vi ber om ursäkt för all förvirring.

1. [Skapa ett nytt ](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) standardprogram och ge det namnet  **Lägg till i Blockeringslista**.
1. Klicka på **Ny** och välj **Ny lokal resurs**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Namnge listan och klicka på **Skapa**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Lägg till alla personer i din **smarta lista** som du vill lägga till i Blockeringslista.

   >[!NOTE]
   >
   >Personer på ditt Blockeringslista får inte några operativa e-postmeddelanden.

   ![](assets/three-6.png)

1. Klicka på **Ny** och välj **Ny smart kampanj**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Ange namnet **Ny smart kampanj**. Klicka på **Skapa**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Dra och släpp **Medlem i smart lista**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Välj den smarta listan som du nyss skapade.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Dra och släpp **Ändra datavärde**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. För **Flöde** anger du **Listblock** för **attributet** och anger **Nytt värde** till **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Välj **Kör en gång** på fliken **Schema**.

   ![](assets/ten.png)

1. Välj **Kör nu** och klicka på **Kör**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   YAY! Dessa personer kommer inte längre att få e-post.

   >[!TIP]
   >
   >Skapa en [utlösande smart kampanj](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) med **Ändra datavärde** med **Listat block är true** för alla personer i framtiden som har attribut som kan blocklist.

