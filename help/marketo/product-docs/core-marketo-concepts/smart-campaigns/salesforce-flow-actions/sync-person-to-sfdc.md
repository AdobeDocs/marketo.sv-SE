---
unique-page-id: 1147027
description: Synkronisera person till SFDC - Marketo Docs - Produktdokumentation
title: Synkronisera person till SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---

# Synkronisera person till SFDC {#sync-person-to-sfdc}

Det här flödessteget infogar personer som skapats av Marketo som leads i Salesforce CRM.

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

1. Som standard tilldelas ledande ägare i det här flödessteget baserat på Salesforce-reglerna för automatisk tilldelning.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >Salesforce kräver att fälten Företag och Efternamn är ifyllda. I annat fall avvisas lead-posten.

1. Du kan ange en specifik Salesforce-användare eller lead-kö som huvudägare.

   ![](assets/sync-person-to-sfdc-2.png)

   När du använder det här flödessteget synkroniseras personen omedelbart som en Salesforce-lead och behöver inte vänta på den vanliga synkroniseringen.

   >[!CAUTION]
   >
   >Salesforce tillåter inte att &quot;Kontakter&quot; tilldelas till lead-köer. I det här fallet skapar Marketo en dubblett av&quot;Lead&quot; i Salesforce.
