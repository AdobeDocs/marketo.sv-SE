---
unique-page-id: 9437340
description: Implementera RTP med Tealium Tag Manager - Marketo Docs - produktdokumentation
title: Implementera RTP med Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Implementera RTP med Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP-taggen.

1. Logga in på ditt Tealium Tag Manager-konto.

1. Gå till fliken Taggar och lägg till taggen för anpassad behållare för team, som finns på fliken Övrigt på Marketplace.

1. I fältet Titel anger du **Marketo RTP** och klicka **Slutför**.

1. Spara ändringarna.

   >[!NOTE]
   >
   >Du behöver inte publicera den nya behållaren än.

1. När profilen har sparats klickar du på ditt namn/din e-postadress i det övre högra hörnet av Tealium iQ-konsolen.

1. På Admin-menyn klickar du på **Hantera mallar** under Kontoadministratör.

1. Välj **Egen tealium-behållare: Marketo RTP** i listrutan för att öppna taggmallen.

1. Logga in på ditt RTP-konto.

1. Gå till Kontoinställningar.

   >[!NOTE]
   >
   >Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 11.

1. Under Domän letar du reda på den relevanta domänen och klickar på **Generera tagg**.

1. Kopiera RTP JavaScript-taggen och klistra in den mellan Start Tag Library Code och End Tag Library Code i Tealium Profile Template.

   >[!NOTE]
   >
   >**Viktiga steg**
   >
   >Ta bort `<!-- RTP tag -->` och `<!-- End of RTP tag -->` -taggar från koden som du placerar i den här filen.
   >
   >Ta bort alla `<script type='text/javascript'>` och `</script>` -taggar från koden som du placerar i den här filen.

1. **Klicka på Spara profilmall** och publicera din nya profil.
