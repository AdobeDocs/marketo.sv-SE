---
unique-page-id: 9438139
description: Lägg till person i Blockeringslista - Marketo Docs - produktdokumentation
title: Lägg till person i Blockeringslista
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Lägg till person i Blockeringslista {#add-person-to-blocklist}

Genom att lägga till personer på Blockeringslista kan de inte ta emot din korrespondens.

1. [Skapa ett nytt standardprogram](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) och namnge **Lägg till i Blockeringslista**.

1. Klicka **Nytt** och markera **Ny lokal resurs**.

   ![](assets/add-person-to-blocklist-1.png)

1. Välj **Smart List**.

   ![](assets/add-person-to-blocklist-2.png)

1. Namnge listan och klicka på **Skapa**.

   ![](assets/add-person-to-blocklist-3.png)

1. Lägg till alla personer i **Smart List** som du vill lägga till i Blockeringslista.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Personer på ditt Blockeringslista får inte några operativa e-postmeddelanden.

1. Gå tillbaka till programmet.

   ![](assets/add-person-to-blocklist-5.png)

1. Klicka **Nytt** och markera **Ny smart kampanj**.

   ![](assets/add-person-to-blocklist-6.png)

1. Namnge **Ny smart kampanj**. Klicka **Skapa**.

   ![](assets/add-person-to-blocklist-7.png)

1. Dra och släpp **Medlem i Smart List**.

   ![](assets/add-person-to-blocklist-8.png)

1. Välj den smarta listan som du nyss skapade.

   ![](assets/add-person-to-blocklist-9.png)

1. Klicka på **Flöde** -fliken. Dra och släpp **Ändra datavärde** Flödesåtgärd.

   ![](assets/add-person-to-blocklist-10.png)

1. I **Attribut** nedrullningsbar markering **Blocklista** och ange **Nytt värde** till **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicka på **Schema** och markera **Kör en gång**.

   ![](assets/add-person-to-blocklist-12.png)

1. Välj **Kör nu** och klicka **Kör**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicka **Kör** igen.

   ![](assets/add-person-to-blocklist-14.png)

Dessa personer kommer inte längre att få e-post.

>[!TIP]
>
>Skapa en [utlösa smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) använda **Ändra datavärde** med **Blocklistan är sann** för alla i framtiden som har attribut som kan blocklist.
