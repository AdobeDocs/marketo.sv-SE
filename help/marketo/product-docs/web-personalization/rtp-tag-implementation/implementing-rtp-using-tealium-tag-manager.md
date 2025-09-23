---
unique-page-id: 9437340
description: Implementera RTP med Tealium Tag Manager - Marketo Docs - produktdokumentation
title: Implementera RTP med Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Implementera RTP med tagghanteraren [!DNL Tealium] {#implementing-rtp-using-tealium-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP-taggen.

1. Logga in på ditt [!DNL Tealium] Tag Manager-konto.

1. Navigera till fliken [!UICONTROL Tags] och lägg till [!UICONTROL Tealium Custom Container Tag], som finns på fliken [!UICONTROL Misc] på Marketplace.

1. I [!UICONTROL Title field] anger du **Marketo RTP** och klickar på **[!UICONTROL Finish]**.

1. Spara ändringarna.

   >[!NOTE]
   >
   >Du behöver inte publicera den nya behållaren än.

1. När profilen har sparats klickar du på ditt namn/din e-postadress i det övre högra hörnet av Tealium iQ-konsolen.

1. Klicka på [!UICONTROL Admin] under **[!UICONTROL Manage Templates]** på menyn [!UICONTROL Account Admin].

1. Välj **[!UICONTROL Tealium Custom Container]: Marketo RTP** i listrutan för att öppna taggmallen.

1. Logga in på ditt RTP-konto.

1. Gå till [!UICONTROL Account Settings].

   >[!NOTE]
   >
   >Om du redan har fått din JavaScript-tagg från supporten fortsätter du till steg 11.

1. Under Domän letar du reda på den relevanta domänen och klickar på **[!UICONTROL Generate Tag]**.

1. Kopiera RTP JavaScript-taggen och klistra in den mellan [!UICONTROL Start Tag Library Code] och [!UICONTROL End Tag Library Code] i Tealium Profile Template.

   >[!NOTE]
   >
   >**Viktiga steg**
   >
   >Ta bort taggarna `<!-- RTP tag -->` och `<!-- End of RTP tag -->` från koden som du placerar i den här filen.
   >
   >Ta bort alla `<script type='text/javascript'>`- och `</script>`-taggar från koden som du monterar i den här filen.

1. Klicka på **[!UICONTROL Save Profile Template]** och publicera din nya profil.
