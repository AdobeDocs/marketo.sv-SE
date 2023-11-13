---
description: Adobe Identity Management Overview - Marketo Docs - Product Documentation
title: Adobe Identity Management - översikt
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Adobe Identity Management - översikt {#adobe-identity-management-overview}

Alla nya Adobe Marketo Engage-prenumerationer (31 juli 2023 eller senare) är integrerade med Adobe Identity Management System. Befintliga Marketo-prenumerationer migreras för närvarande till Adobe Identity Management-systemet vid förnyelser och/eller omkontraktshändelser. Migreringar utanför en händelse för förnyelse eller omtilldelning stöds inte för närvarande.

>[!NOTE]
>
>Marketo Support kan inte tillhandahålla några uppdateringar om Adobe IMS-migrering. Adobe Account Team kommer att nå ut med den beräknade tidslinjen de närmaste månaderna. Mer information finns på [den här artikeln](/help/marketo/product-docs/administration/marketo-with-adobe-identity/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}, and the [Frequently Asked Questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Profilnivåer {#profile-levels}

Adobe Marketo Engage prenumerationer på Adobe Identity Management System har stöd för olika profiler. Följande typer av användarprofiler är relevanta för den här integreringen.

<table>
 <tr>
  <td><strong>Adobe Admin Console systemadministratör</strong></td>
  <td>Ansvarig för att skapa identitetskoncept för Adobe och Marketo Engage i Adobe Admin Console. Beviljad roll vid konfigurationen av Adobe-organisationen.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console produktadministratör</strong></td>
  <td>Ansvarig för att ge användare rätt till Marketo Engage-produkten i Adobe Admin Console. Beviljad roll i Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administratör för Adobe Admin Console produktprofil</strong></td>
  <td>Ansvarig för att administrera användare i en produktprofil. De kan inte hantera användare utanför den specifika profilen. En produktprofiladministratör har inte åtkomst till Marketo-programmet om den inte läggs till i produktprofilen som en användare. Deras roll är fortfarande en standardanvändare (standardarbetsyta om de har fler än en arbetsyta).
</td>
 </tr>
 <tr>
  <td><strong>Produktadministratör för Marketo Engage</strong></td>
  <td>En person som har beviljats tillträde till Marketo Engage med administrativ behörighet. Beviljad roll i Marketo Engage, inte i Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage användare</strong></td>
  <td>En person som har fått tillträde till Marketo Engage. Inga administrativa behörigheter.</td>
 </tr>
</table>

## Vanliga frågor och svar {#faq}

Vanliga frågor [finns här](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Administratörsinställningar](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Lägg till eller ta bort en produktadministratör](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Lägg till eller ta bort en användare](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
