---
unique-page-id: 9438139
description: Lägg till person i Blockeringslista - Marketo Docs - produktdokumentation
title: Lägg till person i Blockeringslista
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Lägg till person i Blockeringslista {#add-person-to-blocklist}

Genom att lägga till personer på Blockeringslista kan de inte ta emot din korrespondens.

1. Skapa ett nytt [standardprogram](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} och ge det namnet&quot;Lägg till i Blockeringslista&quot;.

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

1. Klicka på fliken **[!UICONTROL Flow]**. Dra och släpp **[!UICONTROL Change Data Value]**-flödesåtgärden.

   ![](assets/add-person-to-blocklist-10.png)

1. I listrutan **[!UICONTROL Attribute]** väljer du **[!UICONTROL Block Listed]** och anger **[!UICONTROL New Value]** till **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicka på fliken **[!UICONTROL Schedule]** och välj **[!UICONTROL Run Once]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Markera **[!UICONTROL Run Now]** och klicka på **[!UICONTROL Run]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicka på **[!UICONTROL Run]** igen.

   ![](assets/add-person-to-blocklist-14.png)

Dessa personer kommer inte längre att få e-post.

>[!TIP]
>
>Skapa en [utlösarkampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} med **Ändra datavärde** med **Blocklistan är true** för alla personer i framtiden som har attribut som kan blocklist.
