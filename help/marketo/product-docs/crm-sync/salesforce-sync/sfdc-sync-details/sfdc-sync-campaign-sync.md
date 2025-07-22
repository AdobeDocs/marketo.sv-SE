---
unique-page-id: 2953469
description: SFDC Sync - Campaign Sync - Marketo Docs - Produktdokumentation
title: SFDC Sync - kampanjsynkronisering
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# SFDC Sync: Campaign Sync {#sfdc-sync-campaign-sync}

Marketo-program kan synkroniseras med [!DNL Salesforce] kampanjer. Här är en översikt över hur detta fungerar.

## Varför ska jag synkronisera Marketo-program med [!DNL Salesforce] kampanjer? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utnyttja de kraftfulla funktionerna i Marketo.
* Håll medlemmarna och deras status synkroniserade mellan ett Marketo-program och en [!DNL Salesforce]-kampanj.
* Utnyttja rapportfunktionerna i Marketo och [!DNL Salesforce].

## Hur synkroniseras ett Marketo-program och en [!DNL Salesforce]-kampanj? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

I Marketo kan du skapa en 1:1-mappning mellan ett program och en [!DNL Salesforce]-kampanj.

![](assets/image2015-7-8-9-3a43-3a8.png)

**[Kanalen](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** och **[periodkostnaden](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** i Marketo synkroniseras till [!DNL Salesforce] som **kampanjtypen** och **faktisk kostnad**. Synkroniseringen är **ett sätt**, från Marketo till [!DNL Salesforce].

Marketo **programmedlemmar** och deras **[progressionsstatus](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** synkroniseras med **[!DNL Salesforce]kampanjmedlemmar** och **kampanjmedlemsstatusar**. Detta är en **dubbelriktad synkronisering**, så alla ändringar som görs i antingen Marketo eller [!DNL Salesforce] återspeglas i båda systemen.

>[!NOTE]
>
>Om det finns medlemmar i Marketo-programmet som inte finns i [!DNL Salesforce] skapar Marketo dessa personer som leads i [!DNL Salesforce].

## Vilka utlösare/filter är relaterade till kampanjer? {#what-are-the-triggers-filters-related-to-campaigns}

Utlösare:

* Tillagd i SFDC Campaign
* Borttagen från SFDC Campaign
* Status har ändrats i SFDC Campaign

Filter:

* Medlem i SFDC Campaign

## Kan jag lägga till Marketo People i min SFDC-kampanj? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Ja, använd åtgärden [Lägg till i SFDC kampanjflöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Om den här personen inte finns i [!DNL Salesforce] skapar Marketo den i [!DNL Salesforce] och lägger sedan till honom/henne i kampanjen.

## Kan jag ta bort medlemmar från min SFDC-kampanj med Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Ja, använd flödesåtgärden [Ta bort från SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Kan jag ändra kampanjmedlemmens status med Marketo? {#can-i-change-campaign-member-status-using-marketo}

Ja, använd [Ändra status i SFDC Campaign-flödesåtgärden](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Varför kan jag inte se någon av mina [!DNL Salesforce]-kampanjer? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Här är saker du kan kontrollera:

1. Kontrollera att [kampanjsynkroniseringen är aktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Bekräfta att din [Marketo Sync-användare](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) är en [marknadsföringsanvändare](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) i [!DNL Salesforce].

>[!NOTE]
>
>Om din [!DNL Salesforce]-kampanj och det mappade Marketo-programmet har inkompatibla programstatusvärden kan ett felmeddelande visas. Vi rekommenderar att du [matchar programstatusvärdena före synkroniseringen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Synkronisera en SFDC-kampanj med ett program](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Om programmedlemskap](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Aktivera/inaktivera kampanjsynkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Gör Marketo Sync-användare till marknadsföringsanvändare](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
