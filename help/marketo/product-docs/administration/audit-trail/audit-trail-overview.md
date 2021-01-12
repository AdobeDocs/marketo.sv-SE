---
unique-page-id: 11377945
description: Översikt över granskningsspår - Marketo Docs - Produktdokumentation
title: Översikt över granskningsspår
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Översikt över granskningsspår {#audit-trail-overview}

Granskningsspår ger dig möjlighet att få en komplett historik (värd sex månader) över ändringar som gjorts i din Marketo-instans.

>[!NOTE]
>
>Historiken över granskningsspår började den 14 september 2016.

![](assets/one.png)

## Vad är granskningsspår {#what-is-audit-trail}?

Granskningsspår innehåller i realtid en omfattande lista över åtgärder och händelser som inträffar inom en Marketo-prenumeration. Det innehåller ett självbetjäningssätt att få tillgång till en sexmånadershistorik med data som kan hjälpa dig att svara på frågor som:

Vad hände med den här resursen eller inställningen och vem uppdaterade den senast?

Vad har användare X haft på gång?

Vem loggar in på vårt konto?

## Vad vi granskar {#what-we-audit}

Marketo granskar [skapa, redigera och ta bort](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md)-åtgärder för:

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
>Marketo är _inte_ granskar ändringar som gjorts i Webbpersonalisering, Predictive Content eller Sales Insight just nu.

## Granskningsspårskomponenter {#audit-trail-components}

Granskningsspåret består av tre komponenter.

**1)  [Resursgranskningsspår](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Se aktivitet för specifika resurser.

**2)  [Granskningsspår för administratörer](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Övervaka användarbaserad information.

**3)  [Användarinloggningshistorik](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Se vilka som loggat in på prenumerationen och när. Inkluderar även misslyckade inloggningsförsök.

>[!TIP]
>
>Det finns så mycket du kan granska med granskningsspår att du måste använda [Filtrering](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Exporterar data {#exporting-data}

Du kan bara visa 30 dagars data i din instans. Använd exportalternativet för att få ett värde på upp till sex månader.

![](assets/two.png)

>[!NOTE]
>
>**Definition**
>
>**Okänd:** I granskningsspår kan du se en användares namn och e-postadress som listas som&quot;Okänd&quot;. Det här inträffar när du ändrar värdena i din plocklista i CRM. Dessa värden visas i Marketo-formulär och på landningssidor. Om du gör den här uppdateringen på CRM-sidan läggs dina landningssidor automatiskt till som refererar till formuläret. I granskningsspår kommer vi att se att landningssidan har skrivits, men användarens namn och e-postadress kommer att visas som&quot;Okänd&quot; eftersom vi inte kan samla in användarinformation från CRM-sidan.

>[!MORELIKETHIS]
>
>[Aktivera granskningsspår](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
