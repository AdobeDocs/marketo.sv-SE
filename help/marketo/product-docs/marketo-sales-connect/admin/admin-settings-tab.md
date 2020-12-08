---
unique-page-id: 14352404
description: Fliken Administratörsinställningar - Marketo Docs - Produktdokumentation
title: Fliken Administratörsinställningar
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Fliken Administratörsinställningar {#admin-settings-tab}

På fliken Administratörsinställningar kan administratören för vilket konto som helst både se teamets inställningar (vad gäller planbegränsningar) och masskontrollera hur teamets e-postmeddelanden loggas i Salesforce.

Om du markerar kryssrutan **Åsidosätt alla Salesforce-synkroniseringsinställningar för mitt team** visas alternativet att antingen bara tillåta loggning via BCC eller enbart via API.

Om du väljer **API-loggning**, alla inställningar som är valda för säljprojekt, leads, kontakter `will be set for the entire team after you click **Save Changes**.`

Härifrån kan du också massaktivera säljprojekt och aktivitetssynkronisering i hela teamet.

>[!NOTE]
>
>Om du aktiverar de här inställningarna används ett stort antal API-anrop i teamets Salesforce-inställningar.

1 - Aktivera&quot;Konfigurera mitt teams inställningar&quot;

2 - Aktivera inställningar för teamomfattande synkronisering

3 - Konfigurera hur du vill att din e-postaktivitet och den senaste MSE-aktiviteten ska loggas till SFDC

4 - Aktivera&quot;Synkronisera försäljningskontaktuppgifter&quot; är valfritt

(Obs! MSE gör att du kan hoppa över uppgifter medan SFDC inte gör det, så du måste bestämma hur SFDC hanterar den uppgift som hoppade över)
