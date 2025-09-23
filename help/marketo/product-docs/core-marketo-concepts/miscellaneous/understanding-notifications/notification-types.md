---
unique-page-id: 2953243
description: Meddelandetyper - Marketo Docs - produktdokumentation
title: Meddelandetyper
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---

# Meddelandetyper {#notification-types}

Det finns flera meddelandetyper.

## Kampanjfel  {#campaign-failure}

Kampanjfel meddelar dig om fel i smarta kampanjer.

## CRM-synkronisering {#crm-sync}

CRM-synkroniseringsmeddelanden varnar dig för viktiga problem som har uppstått med CRM-synkroniseringen, till exempel felaktiga behörigheter eller att synkroniseringen är inaktiverad.

**[!DNL Microsoft Dynamics]**

[!DNL Dynamics] meddelanden skickas en gång var 24:e timme och innehåller leads som inte kunde synkroniseras under den tidsperioden. Vanliga orsaker till fel är dubblettleads (som ovan) eller felmatchningar av fältlängd.

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Om du använder [!DNL Salesforce] ser synkroniseringsfelmeddelanden ut ungefär som nedan. Typiska fel är bland annat utgångna autentiseringsuppgifter och API-gränser har överskridits.

![](assets/salesforcesyncerror.png)

## Engagemang {#engagement}

När folk blir utmattade i en ström skickar vi ett meddelande. Anmälan innehåller antalet personer som blivit utmattade och vissa andra uppgifter.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Om du försöker skicka personer till Facebook utan att acceptera användarvillkoren, eller om du försöker skicka personer till Facebook efter att du har tagit bort Marketo-appen.

## Rensa inaktiv utlösarkampanj {#idle-trigger-campaign-cleanup}

Inaktivera utlösta smarta kampanjer som inte längre får någon aktivitet. Läs mer om [automatisk rensning av utlösarkampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

När Marketo inte kan skapa en ny målgrupp loggar du in eller skickar e-post till LinkedIn efter tre försök.

![](assets/linkedin.png)

## Webbtjänster {#web-services}

Du meddelas när du når din dagliga kvot. Kvotmängden återställs varje natt vid midnatt, centraltid.

>[!NOTE]
>
>En del felkoder som du kan få beskrivs i [Utvecklardokumentation](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/error-codes).
