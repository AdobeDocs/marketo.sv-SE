---
unique-page-id: 10095644
description: Godkänn ett utdrag utan utkast - Marketo Docs - produktdokumentation
title: Godkänn ett kodfragment utan utkast
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
feature: Snippets
source-git-commit: 7ea15136c4557b3e651f5ae8a5cda6fcd6b80d1c
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Godkänn ett kodfragment utan utkast {#approve-a-snippet-with-no-draft}

## Godkänn kodavsnittet {#approve-the-snippet}

Inget utkast utlöses varje gång ett fragment godkänns. Detta inkluderar ett fragment som delas eller refereras av resurser i andra arbetsytor.

1. Gå till **[!UICONTROL Design Studio]**.

   ![](assets/approve-the-snippet-1.png)

1. Sök efter och markera önskat fragment.

   ![](assets/approve-the-snippet-2.png)

1. I **[!UICONTROL Snippet actions]** nedrullningsbar meny, välja **[!UICONTROL Approve draft]**.

   ![](assets/approve-the-snippet-3.png)

1. Välj ett alternativ i dialogrutan Godkänn fragment och klicka på **[!UICONTROL Approve]**:

   * **[!UICONTROL Update all]**: Det här alternativet skapar inte utkast av godkända resurser med fragmentet. Alla mediefiler får uppdateringarna och underhåller deras tidigare status. En förloppsmodul visas längst upp till höger på skärmen och kan stängas när som helst. Om du vill återställa fragmentet högerklickar du på fragmentnamnet och väljer Visa godkännandestatus.
   * **[!UICONTROL Create drafts]**: Det här alternativet skapar utkast av godkända resurser med fragmentet. Välj det här alternativet om ändringar av kodfragment måste granskas först. Alla utkast måste godkännas manuellt.

   ![](assets/approve-the-snippet-4.png)

   >[!NOTE]
   >
   >För ett nytt fragment som inte har använts än visas inte skärmen Godkänn utkast. Det visas när fragmentet används i en eller flera resurser.

>[!CAUTION]
>
>Den här funktionen är utformad för att spara tid med arbetsflödet för godkännande av fragment. Det finns dock några begränsningar att vara medveten om. Se [den här artikeln](https://nation.marketo.com/t5/knowledgebase/no-draft-snippet-limitations-and-troubleshooting/ta-p/300799){target="_blank"} för mer information.

>[!MORELIKETHIS]
>
>[Aktivera No-draft för kodfragment](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md){target="_blank"}
