---
unique-page-id: 9438139
description: Lägg till person i Blockeringslista - Marketo Docs - produktdokumentation
title: Lägg till person i Blockeringslista
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 4%

---

# Lägg till person i Blockeringslista {#add-person-to-blocklist}

Genom att lägga till personer på Blockeringslista kan de inte ta emot din korrespondens.

1. Skapa ett nytt [standardprogram](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} och kalla det&quot;Lägg till i Blockeringslista&quot;.

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Local Asset]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Välj **[!UICONTROL Smart List]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Namnge listan och klicka på **[!UICONTROL Create]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Lägg till alla personer i din smarta lista som du vill lägga till i Blockeringslista.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Personer på ditt Blockeringslista får inte några operativa e-postmeddelanden.

1. Gå tillbaka till programmet.

   ![](assets/add-person-to-blocklist-5.png)

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Smart Campaign]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Ge den nya smarta kampanjen ett namn. Klicka på **[!UICONTROL Create]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Dra och släpp **[!UICONTROL Member of Smart List]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Välj den smarta lista du just skapade.

   ![](assets/add-person-to-blocklist-9.png)

1. Klicka på **[!UICONTROL Flow]** -fliken. Dra och släpp **[!UICONTROL Change Data Value]** Flödesåtgärd.

   ![](assets/add-person-to-blocklist-10.png)

1. I **[!UICONTROL Attribute]** nedrullningsbar markering **[!UICONTROL Block Listed]** och ange **[!UICONTROL New Value]** till **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicka på **[!UICONTROL Schedule]** och markera **[!UICONTROL Run Once]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Välj **[!UICONTROL Run Now]** och klicka **[!UICONTROL Run]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicka **[!UICONTROL Run]** igen.

   ![](assets/add-person-to-blocklist-14.png)

Dessa personer kommer inte längre att få e-post.

>[!TIP]
>
>Skapa en [Utlös kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} använda **Ändra datavärde** med **Blocklistan är sann** för alla i framtiden som har attribut som kan blocklist.
