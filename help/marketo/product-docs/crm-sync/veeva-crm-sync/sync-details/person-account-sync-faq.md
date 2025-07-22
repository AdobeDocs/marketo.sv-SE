---
description: Synkronisering av personkonto - frågor och svar - Marketo Docs - produktdokumentation
title: Vanliga frågor om synkronisering av personkonto
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Vanliga frågor om synkronisering av personkonto {#person-account-sync-faq}

Marketo Engage synkroniserar hela databasen med [!DNL Veeva] för personkontotypen för poster. Efter synkroniseringen väntar det 5 minuter och synkroniseras sedan igen, hela dagen, varje dag.

Personkonton kan konfigureras i [!DNL Veeva] för att passa organisationens behov.

>[!NOTE]
>
>Vi synkroniserar bara&quot;Professional&quot;-nivåkonton som personkonton.

**Vad är ett personkonto?**

Ett personkonto liknar kontoobjektet i [!DNL Veeva] CRM. Ett personkonto har dock åtkomst till både kontofält och kontaktfält.

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

Synkroniseringen av kontaktrelaterade fält för personkontot är dubbelriktad. Om du ändrar en kontakt i antingen [!DNL Veeva] CRM eller Marketo återspeglas dina uppdateringar i båda systemen. Fälten på kontot synkroniseras endast i en riktning, från [!DNL Veeva] CRM till Marketo.

**Vad händer om ändringar görs i båda systemen i kontaktfälten på personkontot samtidigt?**

Vi vore trevliga och lät [!DNL Veeva] CRM vinna. Det är dock sällsynt att en sådan kollision mellan data inträffar.

**Är lead- eller kontakttypen för poster synkroniserade med [!DNL Veeva] CRM?**

[!DNL Veeva] CRM hanterar bara objekt för personkonton och har även företagskonton. De traditionella CRM-typerna av lead, kontakter och säljprojekt används inte riktigt i traditionella [!DNL Veeva] CRM-system. Dessa kan ha skapats i [!DNL Veeva] CRM, men stöds inte officiellt med den här kopplingen.

**Kan jag konvertera en person till en kontakt i Marketo?**

Nej, eftersom lead och kontakt inte stöds för synkronisering med [!DNL Veeva] CRM. Därför stöds inte konvertering.

**Kan jag framtvinga en synkronisering av en kontakt manuellt?**

Nej, eftersom Kontakt inte är en oberoende typ av post stöds inte synkronisering av en person till [!DNL Veeva].

**Synkroniserar varje standardfält med Marketo?**

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som din Marketo Sync-användare har åtkomst till.

**Kommer Marketo att respektera [!DNL Veeva]-valideringsreglerna?**

Ja, om en konflikt uppstår loggar vi resultatet i leadets aktivitetslogg.

>[!MORELIKETHIS]
>
>* [Standard [!DNL Veeva] Fältmappning](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Synkroniserar meddelande för samtal och samtal](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
