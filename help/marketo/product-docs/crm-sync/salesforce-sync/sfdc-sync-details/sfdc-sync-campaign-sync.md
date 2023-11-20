---
unique-page-id: 2953469
description: SFDC-synkronisering - Kampanjsynkronisering - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - kampanjsynkronisering
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# SFDC-synkronisering: Kampanjsynkronisering {#sfdc-sync-campaign-sync}

Marketo Engage-program kan synkroniseras med Salesforce-kampanjer. Här är en översikt över hur detta fungerar.

## Varför ska jag synkronisera Marketo-program med Salesforce-kampanjer? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utnyttja de kraftfulla funktionerna i Marketo.
* Håll medlemmarna och deras status synkroniserade mellan ett Marketo-program och en Salesforce-kampanj.
* Utnyttja rapportfunktionerna i Marketo och Salesforce.

## Hur synkroniseras ett Marketo-program och en Salesforce-kampanj? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

I Marketo kan du skapa en mappning mellan ett program och en Salesforce-kampanj.

![](assets/image2015-7-8-9-3a43-3a8.png)

The **[kanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}** and **[period cost](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md){target="_blank"}** i Marketo synkronisera med Salesforce som **kampanjtyp** och **faktisk kostnad**. Synkroniseringen är **ett sätt**, från Marketo till Salesforce.

Marketo **programmedlemmar** och **[förloppsstatus](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}** synkroniseras med **Salesforce-kampanjmedlemmar** och **kampanjmedlemsstatus**. Det här är en **dubbelriktad synkronisering** så att alla ändringar som görs i antingen Marketo eller Salesforce återspeglas i båda systemen.

>[!NOTE]
>
>Om det finns medlemmar i Marketo-programmet som inte finns i Salesforce skapar Marketo dessa personer som leads i Salesforce.

## Vilka utlösare/filter är relaterade till kampanjer? {#what-are-the-triggers-filters-related-to-campaigns}

Utlösare:

* Tillagd i SFDC-kampanj
* Borttagen från SFDC-kampanj
* Status har ändrats i SFDC-kampanj

Filter:

* Medlem i SFDC Campaign

## Kan jag lägga till Marketo People i min SFDC-kampanj? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Ja, använd [Lägg till i SFDC-kampanjflödesåtgärd](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md){target="_blank"}. Om den här personen inte finns i Salesforce skapar Marketo den i Salesforce och lägger sedan till honom/henne i kampanjen.

## Kan jag ta bort medlemmar från min SFDC-kampanj med Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Ja, använd [Åtgärd för att ta bort från SFDC-kampanjflöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Kan jag ändra kampanjmedlemmens status med Marketo? {#can-i-change-campaign-member-status-using-marketo}

Ja, använd [Ändra status i SFDC-kampanjflödesåtgärd](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Varför kan jag inte se någon av mina Salesforce-kampanjer? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Här är saker du kan kontrollera:

1. Se till att [kampanjsynkronisering är aktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
1. Bekräfta att [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} is a [Marketing User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} i Salesforce.

>[!NOTE]
>
>Om Salesforce-kampanjen och det mappade Marketo-programmet har inkompatibla programstatusvärden kan ett felmeddelande visas. Vi rekommenderar att du [matchar programstatusvärdena före synkroniseringen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Synkronisera en SFDC-kampanj med ett program](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Förstå programmedlemskap](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Aktivera/inaktivera kampanjsynkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Gör Marketo Sync User till marknadsföringsanvändare](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
