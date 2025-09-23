---
unique-page-id: 1147074
description: Automatisk rensning av utlösningskampanj - Marketo Docs - produktdokumentation
title: Automatisk rensning av utlösarkampanj
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Automatisk rensning av utlösarkampanj {#automatic-trigger-campaign-cleanup}

Marketo har en fin/kostnadsfri tjänst för att inaktivera utlösta smarta kampanjer som inte längre får aktivitet. Detta snabbar upp den övergripande systemprestandan och sparar tid.

## Vad händer? {#what-happens}

En gång i kvartalet kommer Marketo att hitta smarta kampanjer som har stannat (inga personer) i sex månader eller mer och inaktivera dem.

## Kan du meddela mig först? {#will-you-notify-me-first}

Självklart! En gång per kvartal får ni ett meddelande en vecka i förväg med alla kampanjer vi planerar att inaktivera.

1. Klicka på ikonen **[!UICONTROL Notifications]**.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Klicka på **[!UICONTROL Idle Trigger Campaign Cleanup Scheduled]**. Klicka sedan på länken **[!UICONTROL These Idle Trigger Campaigns will be deactivated]**.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Du ser en lista över smarta kampanjer som är schemalagda att inaktiveras.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## Vilka kampanjer kommer att inaktiveras? {#which-campaigns-will-be-deactivated}

Vi inaktiverar bara utlösarkampanjer som har varit aktiva i över sex månader men har haft 0 personer kvalificerade under den perioden.

## Vänta! Inte den här kampanjen! {#wait-not-this-campaign}

Oroa dig inte - klockan på Smart Campaign kan återställas genom att:

* En person som kvalificerar sig för kampanjen.
* Inaktivera och återaktivera kampanjen manuellt.

Antingen återställs 6-månadersräknaren.

## Kan du meddela mig vilka kampanjer som inaktiverats? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolut - en vecka efter det ursprungliga meddelandet inaktiverar vi de listade kampanjerna (minus alla som kvalificerat minst en person eller inaktiverats/återaktiverats) och skickar ett bekräftelsemeddelande.

1. Välj meddelandet **[!UICONTROL Idle Trigger Campaign Cleanup Scheduled]**. Klicka på länken **[!UICONTROL These Idle Trigger Campaigns]**.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. En lista över inaktiverade kampanjer visas.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
