---
unique-page-id: 1147027
description: Synkronisera person till SFDC - Marketo Docs - Produktdokumentation
title: Synkronisera person till SFDC
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Synkronisera person till SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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

