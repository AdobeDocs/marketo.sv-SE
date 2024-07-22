---
unique-page-id: 4719291
description: Ange standardperson, efternamn och företagsnamn - Marketo Docs - produktdokumentation
title: Ange standardpersonens efternamn och företagsnamn
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---

# Ange standardpersonens efternamn och företagsnamn {#set-default-person-last-name-and-company-name}

Salesforce kräver (minimum) efternamn och företagsnamn för sina leads och kontakter. Ofullständiga poster synkroniseras inte till Salesforce. Om du vill synkronisera partiella poster måste du ange standardvärden för Marketo som ska användas med Salesforce.

1. Gå till **[!UICONTROL Admin]** och klicka på **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Klicka på **[!UICONTROL Edit Sync Options]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Ange en **[!UICONTROL Default person last name]** och en **[!UICONTROL Default person company]** och klicka sedan på **[!UICONTROL Save]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage tilldelar bara ett standardvärde när posten först synkroniseras med Salesforce, och bara om något av de obligatoriska fälten är tomt.

Och det där! Varje gång en person saknar efternamn och/eller företagsnamn lägger Marketo till standardvärdet när posten synkroniseras.
