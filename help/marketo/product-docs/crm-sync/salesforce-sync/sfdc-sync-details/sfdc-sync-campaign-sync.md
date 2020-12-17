---
unique-page-id: 2953469
description: SFDC Sync -Campaign Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Kampanjsynkronisering
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# SFDC-synkronisering: Kampanjsynkronisering {#sfdc-sync-campaign-sync}

Marketo-program kan synkroniseras med Salesforce-kampanjer. Här är en översikt över hur detta fungerar.

## Varför ska jag synkronisera Marketo-program med Salesforce-kampanjer? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Använd de kraftfulla funktionerna i ett Marketo-program.
* Håll medlemmarna och deras status synkroniserade mellan ett Marketo-program och en Salesforce-kampanj.
* Utnyttja rapportfunktionerna i Marketo och Salesforce.

## Hur synkroniseras ett Marketo-program och en Salesforce-kampanj? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

I Marketo kan du skapa en personlig mappning mellan ett program och en Salesforce-kampanj.

![](assets/image2015-7-8-9-3a43-3a8.png)

** [channel](../../../../product-docs/administration/tags/create-a-program-channel.md) **och ** [periodkostnad](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** i Marketför att synkronisera till Salesforce som **kampanjtyp** och **faktisk kostnad**. Den här synkroniseringen är **ett sätt**, från Marketo till Salesforce.

Marketo **programmedlemmar** och deras ** [progressionsstatus](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** är synkroniserade med Salesforce-kampanjmedlemmarna **och** kampanjmedlemsstatyer **.** Detta är en **dubbelriktad** **synkronisering**, så alla ändringar som görs i Marketo eller Salesforce återspeglas i båda systemen.

>[!NOTE]
>
>Om det finns medlemmar i Marketo-programmet som inte finns i Salesforce, skapar Marketo dessa personer som leads i Salesforce.

## Vilka utlösare/filter hör till kampanjer? {#what-are-the-triggers-filters-related-to-campaigns}

Utlösare:

* Tillagd i SFDC-kampanj
* Borttagen från SFDC-kampanj
* Status har ändrats i SFDC-kampanj

Filter:

* Medlem i SFDC Campaign

## Kan jag lägga till Marketo People i min SFDC-kampanj? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Ja, använd åtgärden [Lägg till i SFDC-kampanjflöde](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Om den här personen inte finns i Salesforce skapar Marketo den i Salesforce och lägger sedan till honom/henne i kampanjen.

## Kan jag ta bort medlemmar från min SFDC-kampanj med Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Ja, använd åtgärden [Ta bort från SFDC Campaign-flödet](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## Kan jag ändra kampanjmedlemmens status med Marketo? {#can-i-change-campaign-member-status-using-marketo}

Ja, använd åtgärden [Ändra status i SFDC Campaign-flödesåtgärden](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Varför kan jag inte se någon av mina Salesforce-kampanjer? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Här är saker du kan kontrollera:

1. Kontrollera att [kampanjsynkroniseringen är aktiverad](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Bekräfta att din [Marketo Sync-användare](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) är en [marknadsföringsanvändare](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) i Salesforce.

>[!NOTE]
>
>Om Salesforce-kampanjen och det mappade Marketo-programmet har inkompatibla programstatusar kan ett felmeddelande visas. Vi rekommenderar att du [matchar programstatusvärdena före synkroniseringen](sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Synkronisera en SFDC-kampanj med ett program](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Förstå programmedlemskap](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Aktivera/inaktivera kampanjsynkronisering](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Gör Marketo till Sync User a Marketing User](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

>



