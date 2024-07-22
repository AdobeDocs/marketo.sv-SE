---
unique-page-id: 9437340
description: Implementera RTP med Tealium Tag Manager - Marketo Docs - produktdokumentation
title: Implementera RTP med Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Implementera RTP med Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP-taggen.

1. Logga in på ditt Tealium Tag Manager-konto.

1. Gå till fliken Taggar och lägg till taggen för anpassad behållare för team, som finns på fliken Övrigt på Marketplace.

1. Ange **Marketo RTP** i fältet Titel och klicka på **Slutför**.

1. Spara ändringarna.

   >[!NOTE]
   >
   >Du behöver inte publicera den nya behållaren än.

1. När profilen har sparats klickar du på ditt namn/din e-postadress i det övre högra hörnet av Tealium iQ-konsolen.

1. Klicka på **Hantera mallar** under Kontoadministratör på Admin-menyn.

1. Välj **Anpassad behållare för team: Marketo RTP** i listrutan för att öppna taggmallen.

1. Logga in på ditt RTP-konto.

1. Gå till Kontoinställningar.

   >[!NOTE]
   >
   >Om du redan har fått din JavaScript-tagg från supporten fortsätter du till steg 11.

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

1. Kopiera RTP JavaScript-taggen och klistra in den mellan starttaggsbibliotekskoden och sluttaggbibliotekskoden i Tealium Profile Template.

   >[!NOTE]
   >
   >**Viktiga steg**
   >
   >Ta bort taggarna `<!-- RTP tag -->` och `<!-- End of RTP tag -->` från koden som du placerar i den här filen.
   >
   >Ta bort alla `<script type='text/javascript'>`- och `</script>`-taggar från koden som du monterar i den här filen.

1. **Klicka på Spara profilmall** och publicera den nya profilen.
