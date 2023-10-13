---
unique-page-id: 1147091
description: Understanding Program Membership - Marketo Docs - Product Documentation
title: Förstå programmedlemskap
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 86f9e9f13b24a82deb50ec4c398035d7d7479d20
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Förstå programmedlemskap {#understanding-program-membership}

>[!NOTE]
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/person i våra dokument. De här termerna betyder samma sak; de påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md){target="_blank"}.

>[!NOTE]
>
>**Definition:** En medlem är en person som har status i ett program.

## Så här blir människor medlemmar i ett program {#how-people-become-members-of-a-program}

1. En person fyller i en [formulär på en landningssida](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} i programmet.

   1. Personen får automatiskt den första statusen i förloppet.

1. Du [importera medlemmar till programmet](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"} från en CSV-fil.

   1. Personen får automatiskt den första statusen i förloppet.

1. Du använder [ändra programstatus](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"} flödessteg.
1. En person registrerar eller deltar i en [webbinarium synkroniserat med ett händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md){target="_blank"}.
1. En person är [som skapats med incheckningsprogrammet för Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md){target="_blank"}.
1. En person läggs till i en SFDC-kampanj, som är [synkad till programmet](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}.

>[!NOTE]
>
>För ett e-postprogram läggs en person till i medlemskapet endast när e-postmeddelandet skickas.

## Programstatus {#program-statuses}

Programstatus är de steg som användarna går igenom i ett program (t.ex. Inbjuden, RSVP&#39;d, Attended, No Show). Dessa steg definieras av [kanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>En person kan inte gå tillbaka till en tidigare programstatus. Statusutvecklingen är bara ett sätt.

## Slutförandestatus {#success-statuses}

Syftet med ett program är att skapa en meningsfull interaktion med personen eller den potentiella kunden. Lyckade markeras när en person når den status som uppnår det målet.

>[!NOTE]
>
>För ett webbinarium är registrering inte en meningsfull interaktion om de inte tittar på webbinariet. Att delta är lyckat i det här fallet.

## Anskaffningsprogram {#acquisition-program}

När ett nytt namn kommer in i systemet som programmedlem anger Marketo automatiskt det programmet som&quot;förvärv&quot;. Detta skapar kredit för [Första kontakten-attribuering](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Använd taggar i ett program](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md){target="_blank"}
>* [Skapa en rapport om programprestanda](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md){target="_blank"}
