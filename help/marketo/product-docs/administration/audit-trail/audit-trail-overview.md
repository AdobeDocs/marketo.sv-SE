---
unique-page-id: 11377945
description: Översikt över granskningsspår - Marketo Docs - Produktdokumentation
title: Översikt över granskningsspår
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Översikt över granskningsspår {#audit-trail-overview}

Granskningsspår ger dig möjlighet att få en komplett historik (värd sex månader) över ändringar som gjorts i din Marketo-instans.

>[!NOTE]
>
>Historiken över granskningsspår började den 14 september 2016.

![](assets/one.png)

## Vad är granskningsspår? {#what-is-audit-trail}

Granskningsspår innehåller i realtid en omfattande lista över åtgärder och händelser som inträffar inom en Marketo-prenumeration. Det innehåller ett självbetjäningssätt att få tillgång till en sexmånadershistorik med data som kan hjälpa dig att svara på frågor som:

Vad hände med den här resursen eller inställningen och vem uppdaterade den senast?

Vad har användare X haft på gång?

Vem loggar in på vårt konto?

## Vad vi granskar {#what-we-audit}

Marketo granskar [skapa, redigera och ta bort](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) åtgärder för:

* Designstudiematerial
* Alla Marketo-program
* Smarta kampanjer
* Listor (smart/statisk)
* Användare (admin)
* Roller och behörigheter (administratör)
* Arbetsyta och partitioner (admin)
* Användarinloggningshistorik

>[!NOTE]
>
>Marketo granskar **inte** ändringar som gjorts i Webbpersonalisering, Predictive Content eller Sales Insight.

## Granskningsspårskomponenter {#audit-trail-components}

Granskningsspåret består av tre komponenter.

**1) [Resursgranskningsspår](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

Se aktivitet för specifika resurser.

**2) [Granskningsspår för administratörer](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

Övervaka användarbaserad information.

**3) [Användarinloggningshistorik](http://docs.marketo.com/display/DOCS/User+Login+History)**

Se vilka som loggat in på prenumerationen och när. Inkluderar även misslyckade inloggningsförsök.

>[!TIP]
>
>Det finns så mycket du kan granska med granskningsspår, se till att använda [filtrering](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## Exporterar data {#exporting-data}

Du kan bara visa 30 dagars data i din instans. Använd exportalternativet för att få ett värde på upp till sex månader.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Okänd:** I granskningsspår kan du se en användares namn och e-postadress som är&quot;Okänd&quot;. Det här inträffar när du ändrar värdena i din plocklista i CRM. Dessa värden visas i Marketo-formulär och på landningssidor. Om du gör den här uppdateringen på CRM-sidan läggs dina landningssidor automatiskt till som refererar till formuläret. I granskningsspår kommer vi att se att landningssidan har skrivits, men användarens namn och e-postadress kommer att visas som&quot;Okänd&quot; eftersom vi inte kan samla in användarinformation från CRM-sidan.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Aktivera granskningsspår](enable-audit-trail.md)

>



