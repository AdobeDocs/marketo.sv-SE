---
unique-page-id: 1147074
description: Automatisk rensning av kampanjrensning - Marketo Docs - Produktdokumentation
title: Automatisk rensning av utlösarkampanj
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---


# Automatisk rensning av utlösarkampanj {#automatic-trigger-campaign-cleanup}

Marketo har en trevlig/kostnadsfri tjänst för att inaktivera utlösta smarta kampanjer som inte längre får aktivitet. Detta snabbar upp den övergripande systemprestandan och sparar tid.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Vad händer? {#what-happens}

En gång i kvartalet kommer Marketo att hitta smarta kampanjer som har stannat (inga personer) i sex månader eller mer och inaktivera dem.

## Kan du meddela mig först? {#will-you-notify-me-first}

Självklart! En gång per kvartal får ni ett meddelande en vecka i förväg med alla kampanjer vi planerar att inaktivera.

1. Gå till fliken **Meddelanden** .

   ![](assets/notifications.png)

1. Klicka på **Inaktiv utlösare för kampanjrensning schemalagd**. Klicka sedan på **länken **Dessa inaktiva utlösarkampanjer inaktiveras.** **

   ![](assets/image2015-4-27-20-3a48-3a35.png)

   En lista över smarta kampanjer som ska inaktiveras visas.

   ![](assets/image2015-4-27-20-3a35-3a29.png)

## Vilka kampanjer kommer att inaktiveras? {#which-campaigns-will-be-deactivated}

Vi inaktiverar bara utlösarkampanjer som har varit aktiva i över sex månader men har haft 0 personer kvalificerade under den perioden.

## Vänta! Inte den här kampanjen! {#wait-not-this-campaign}

Oroa dig inte - klockan på smarta kampanjer kan återställas med:

* En person som kvalificerar sig för kampanjen.
* Inaktivera och återaktivera kampanjen manuellt.

Antingen återställs 6-månadersräknaren.

## Kan du meddela mig vilka kampanjer som inaktiverats? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolut - en vecka efter det ursprungliga meddelandet inaktiverar vi de listade kampanjerna (minus alla som kvalificerat minst en person eller inaktiverats/återaktiverats) och skickar ett bekräftelsemeddelande.

1. Välj meddelandet **Inaktiv utlösare för kampanjrensning som schemalagts **i. Klicka på länken **Dessa inaktiva utlösarkampanjer** .

   ![](assets/image2015-4-27-20-3a56-3a41.png)

1. En lista över inaktiverade kampanjer visas.

   ![](assets/image2015-4-27-20-3a58-3a38.png)

