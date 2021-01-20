---
unique-page-id: 1147027
description: Synkronisera person till SFDC - Marketo Docs - Produktdokumentation
title: Synkronisera person till SFDC
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Synkronisera person till SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

## Översikt {#overview}

I det här flödessteget infogas Marketo-skapade personer som leads i Salesforce CRM.

![](assets/sync-person-to-sfdc.png)

## Användning {#usage}

1. Som standard tilldelas ledande ägare i det här flödessteget baserat på Salesforce-reglerna för automatisk tilldelning.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce kräver att fälten Företag och Efternamn är ifyllda. I annat fall avvisas lead-posten.

1. Du kan ange en specifik Salesforce-användare eller lead-kö som huvudägare.

   ![](assets/sync-person-to-sfdc-2.png)

   När du använder det här flödessteget synkroniseras personen omedelbart som en Salesforce-lead och behöver inte vänta på den vanliga synkroniseringen.

   >[!CAUTION]
   >
   >Salesforce tillåter inte att &quot;Kontakter&quot; tilldelas till lead-köer. I det här fallet skapar Marketo en dubblett av&quot;Lead&quot; i Salesforce.
