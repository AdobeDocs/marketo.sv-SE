---
unique-page-id: 2953243
description: Meddelandetyper - Marketo Docs - produktdokumentation
title: Meddelandetyper
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Meddelandetyper {#notification-types}

Det finns flera meddelandetyper.

## Kampanjfel  {#campaign-failure}

Kampanjfel meddelar dig om fel i smarta kampanjer.

## CRM-synkronisering {#crm-sync}

CRM-synkroniseringsmeddelanden varnar dig för viktiga problem som har uppstått med CRM-synkroniseringen, till exempel felaktiga behörigheter eller att synkroniseringen är inaktiverad.

**[!DNL Microsoft Dynamics]**

Dynamics-meddelanden skickas en gång var 24:e timme och innehåller leads som inte kunde synkroniseras under den tidsperioden. Vanliga orsaker till fel är dubblettleads (som ovan) eller felmatchningar av fältlängd.

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Om du använder Salesforce ser felmeddelanden ut ungefär som de nedan. Typiska fel är bland annat utgångna autentiseringsuppgifter och API-gränser har överskridits.

![](assets/salesforcesyncerror.png)

## Engagemang {#engagement}

När folk blir utmattade i en ström skickar vi ett meddelande. Anmälan innehåller antalet personer som blivit utmattade och vissa andra uppgifter.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Om du försöker skicka personer till Facebook utan att godkänna användarvillkoren eller om du försöker skicka personer till Facebook efter att du har tagit bort Marketo-appen.

## Rensa inaktiv utlösarkampanj {#idle-trigger-campaign-cleanup}

Inaktivera utlösta smarta kampanjer som inte längre får någon aktivitet. Läs mer om  [automatisk rensning av utlösarkampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

När Marketo inte kan skapa en ny publik, logga in eller skicka e-post till LinkedIn efter tre försök.

![](assets/linkedin.png)

## Webbtjänster {#web-services}

Du meddelas när du når din dagliga kvot. Kvotmängden återställs varje natt vid midnatt, centraltid.

>[!NOTE]
>
>En del felkoder som du kan få beskrivs i våra [Dokumentation för utvecklare](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/error-codes).
