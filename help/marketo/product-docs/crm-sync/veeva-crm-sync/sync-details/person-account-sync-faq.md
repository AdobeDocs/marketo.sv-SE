---
description: Synkronisering av personkonto - frågor och svar - Marketo Docs - produktdokumentation
title: Vanliga frågor om synkronisering av personkonto
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Vanliga frågor om synkronisering av personkonto {#person-account-sync-faq}

Marketo Engage synkroniserar hela databasen med Veeva för personkontotypen. Efter synkroniseringen väntar det 5 minuter och synkroniseras sedan igen, hela dagen, varje dag.

Personkonton kan konfigureras i Veeva för att passa organisationens behov.

>[!NOTE]
>
>Vi synkroniserar bara&quot;Professional&quot;-nivåkonton som personkonton.

**Vad är ett personkonto?**

Ett personkonto liknar kontoobjektet i Veeva CRM. Ett personkonto har dock åtkomst till både kontofält och kontaktfält.

**Vad händer när ett personkonto synkroniseras med Marketo?**

Ett personkonto synkroniseras till Marketo som ett företag och som en person.

>[!NOTE]
>
>De anpassade fälten för ett personkonto kopieras till både företag och person i Marketo.

**Hur skiljer jag på affärskonton och personkonton?**

Använd filtret &quot;Är person&quot;-konto i din smarta lista för att skilja personkonton från vanliga affärskonton.

**Vilket e-postfält ska jag använda för personkonton?**

Det finns två e-postfält för ett personkonto. Använd fältet E-postadress i dina formulär (inte personens e-postadress) för att säkerställa att Marketo kan ta bort dubbletter och annan e-postbearbetning fungerar som den ska.

## Synkroniseringsriktning {#sync-direction}

Synkroniseringen av kontaktrelaterade fält för personkontot är dubbelriktad. Om du ändrar en kontakt i Veeva CRM eller Marketo återspeglas dina uppdateringar i båda systemen. Fälten på kontot synkroniseras endast i en riktning, från Veeva CRM till Marketo.

**Vad händer om ändringar görs i båda systemen i kontaktfälten på personkontot samtidigt?**

Vi vore trevliga och lät Veeva CRM vinna. Det är dock sällsynt att en sådan kollision mellan data inträffar.

**Synkroniseras lead- eller kontakttypen för poster med Veeva CRM?**

Veeva CRM hanterar bara objekt för personkonton och har även företagskonton. De traditionella CRM-typerna av lead, kontakter och säljprojekt används inte i praktiken i traditionella Veeva CRM-system. Dessa kan ha skapats i Veeva CRM, men stöds inte officiellt med den här kopplingen.

**Kan jag konvertera en person till en kontakt i Marketo?**

Nej, eftersom Lead och Kontakt inte stöds för synkronisering med Veeva CRM. Därför stöds inte konvertering.

**Kan jag framtvinga en synkronisering av en kontakt manuellt?**

Nej, eftersom Kontakt inte är en oberoende typ av post stöds inte synkronisering av en person till Veeva.

**Synkroniserar alla standardfält med Marketo?**

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som din Marketo Sync-användare har åtkomst till.

**Kommer Marketo att respektera valideringsreglerna för Veeva?**

Ja, om en konflikt uppstår loggar vi resultatet i leadets aktivitetslogg.

>[!MORELIKETHIS]
>
>* [Standardvevektorgrafikmappning](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Synkronisera samtal och ringa nyckelmeddelanden](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
