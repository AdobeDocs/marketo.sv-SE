---
unique-page-id: 1147074
description: Automatisk rensning av kampanjrensning - Marketo Docs - produktdokumentation
title: Automatisk rensning av utlösarkampanj
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Automatisk rensning av utlösarkampanj {#automatic-trigger-campaign-cleanup}

Marketo har en trevlig/kostnadsfri tjänst för att inaktivera utlösta smarta kampanjer som inte längre får aktivitet. Detta snabbar upp den övergripande systemprestandan och sparar tid.

## Vad händer? {#what-happens}

En gång i kvartalet kommer Marketo att hitta smarta kampanjer som har stannat (inga personer) i minst sex månader och inaktivera dem.

## Kan du meddela mig först? {#will-you-notify-me-first}

Självklart! En gång per kvartal får ni ett meddelande en vecka i förväg med alla kampanjer vi planerar att inaktivera.

1. Klicka på **Meddelanden** ikon.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Klicka **Schemalagd rensning av inaktiv utlösarkampanj**. Klicka sedan på **Dessa inaktiva utlösarkampanjer kommer att inaktiveras** länk.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   En lista över smarta kampanjer som ska inaktiveras visas.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## Vilka kampanjer kommer att inaktiveras? {#which-campaigns-will-be-deactivated}

Vi inaktiverar bara utlösarkampanjer som har varit aktiva i över sex månader men har haft 0 personer kvalificerade under den perioden.

## Vänta! Inte den här kampanjen! {#wait-not-this-campaign}

Oroa dig inte - klockan på smarta kampanjer kan återställas med:

* En person som kvalificerar sig för kampanjen.
* Inaktivera och återaktivera kampanjen manuellt.

Antingen återställs 6-månadersräknaren.

## Kan du meddela mig vilka kampanjer som inaktiverats? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolut - en vecka efter det ursprungliga meddelandet inaktiverar vi de listade kampanjerna (minus alla som kvalificerat minst en person eller inaktiverats/återaktiverats) och skickar ett bekräftelsemeddelande.

1. Välj **Schemalagd rensning av inaktiv utlösarkampanj** meddelande. Klicka på **Dessa inaktiva utlösarkampanjer** länk.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. En lista över inaktiverade kampanjer visas.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
