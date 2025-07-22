---
unique-page-id: 1147027
description: Synkronisera person till SFDC - Marketo Docs - produktdokumentation
title: Synkronisera person till SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---

# Synkronisera person till SFDC {#sync-person-to-sfdc}

Det här flödessteget infogar personer som skapats av Marketo som leads i din Salesforce CRM.

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med [!DNL Salesforce].

1. Som standard tilldelas huvudägare i det här flödessteget baserat på Salesforce regler för automatisk tilldelning.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] kräver att fälten Företag och Efternamn är ifyllda. I annat fall avvisas lead-posten.

1. Du kan ange en specifik [!DNL Salesforce]-användare eller lead-kö som huvudägare.

   ![](assets/sync-person-to-sfdc-2.png)

   När du använder det här flödessteget synkroniseras personen omedelbart som en [!DNL Salesforce]-lead och behöver inte vänta på den vanliga synkroniseringen.

   >[!CAUTION]
   >
   >[!DNL Salesforce] tillåter inte att Kontakter tilldelas till lead-köer. I det här fallet skapar Marketo en dubblett av&quot;Lead&quot; i [!DNL Salesforce].
