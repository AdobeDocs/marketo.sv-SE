---
unique-page-id: 4719291
description: Ange standardperson, efternamn och företagsnamn - Marketo-dokument - produktdokumentation
title: Ange standardpersonens efternamn och företagsnamn
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# Ange standardpersonens efternamn och företagsnamn {#set-default-person-last-name-and-company-name}

Salesforce kräver (minimum) efternamn och företagsnamn för sina leads och kontakter. Ofullständiga poster synkroniseras inte till Salesforce. Om du vill synkronisera partiella poster måste du ange standardvärden för Marketo som ska användas med Salesforce.

1. Gå till **Admin** och klicka på **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Klicka på **Redigera synkroniseringsalternativ**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Ange ett **standardpersonefternamn** och ett **Default ****personföretag** och klicka sedan på **Spara**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo tilldelar bara ett standardvärde när posten först synkroniseras med Salesforce, och bara om något av de obligatoriska fälten är tomt.

Och det där! Varje gång en person saknar efternamn och/eller företagsnamn lägger Marketo till standardvärdet när posten synkroniseras.
