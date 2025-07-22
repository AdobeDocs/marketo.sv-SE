---
unique-page-id: 2953457
description: SFDC Sync - Contact Sync - Marketo Docs - produktdokumentation
title: SFDC Sync - kontaktsynkronisering
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# SFDC Sync: Kontakta Sync {#sfdc-sync-contact-sync}

Visste du att Marketo synkroniserar hela databasen med [!DNL Salesforce]? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar [!DNL Salesforce] kontakter.

## Synkroniseringsriktning {#sync-direction}

Kontaktsynkroniseringen är dubbelriktad. Om du ändrar en kontakt i antingen [!DNL Salesforce] eller Marketo återspeglas dina uppdateringar i båda systemen.

## Vad händer om ändringar görs i båda systemen samtidigt? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Vi är trevliga och låter [!DNL Salesforce] vinna. Det är sällsynt att en sådan kollision mellan data inträffar.

## Kan jag konvertera en person till en kontakt i Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Ja, använd flödesåtgärden **[Konvertera person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>Om du konverterar en person i Marketo skapas ett nytt konto och en ny affärsmöjlighet i [!DNL Salesforce]. Om du inte vill ha dubblettkonton använder du [!DNL Salesforce] för att konvertera.

## Kan jag framtvinga en synkronisering av en kontakt manuellt? {#can-i-manually-force-a-sync-of-a-contact}

Ja, använd flödesåtgärden **[Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** så synkroniseras den i realtid.

## Synkroniserar alla standardfält med Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som din Marketo Sync-användare har åtkomst till.

## Kommer Marketo att respektera verifieringsreglerna för [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, om det finns en konflikt loggas resultatet i lead-aktivitetsloggen.
