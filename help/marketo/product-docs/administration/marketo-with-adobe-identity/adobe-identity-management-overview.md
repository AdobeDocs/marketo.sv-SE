---
description: Adobe Identity Management Overview - Marketo Docs - produktdokumentation
title: Adobe Identity Management - översikt
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Adobe Identity Management - översikt {#adobe-identity-management-overview}

Alla nya Adobe Marketo Engage-prenumerationer (31 juli 2023 eller senare) är integrerade med Adobe Identity Management System. Befintliga Marketo Engage-prenumerationer migreras för närvarande till Adobe Identity Management System vid alla försäljningsevenemang, inklusive förnyelser, omavtalsevenemang och/eller tillägg. Migreringar utanför ett försäljningsevenemang stöds från och med oktober 2024. Marketo-administratörer får ett meddelande 2-4 veckor i förväg om deras prenumeration är planerad att migreras utanför en försäljningshändelse.

>[!NOTE]
>
>Marketo Support kan inte tillhandahålla några uppdateringar om Adobe IMS-migrering. Adobe Account Team kommer att nå ut med den beräknade tidslinjen de närmaste månaderna. Mer information finns i [den här artikeln](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} och i [Vanliga frågor](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

För prenumerationer som är kopplade till Adobe identitet används Adobe Admin Console för användarhantering. Identitetsrelaterade begrepp, som enkel inloggning, hanteras också i Admin Console.

* Mer information om [Adobe Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html){target="_blank"} finns.
* Mer information om [hur du konfigurerar din Adobe-organisation för din Marketo-prenumeration](https://helpx.adobe.com/se/enterprise/using/set-up-identity.html){target="_blank"} finns.

>[!NOTE]
>
>Om du vill implementera enkel inloggning och din prenumeration har registrerats på Adobe Identity utan enkel inloggning (SSO) implementerat i Adobe Org skickar du en biljett till [Marketo Support](https://nation.marketo.com/){target="_blank"} och anger ämnet som&quot;Marketo on Admin Console, implement SSO&quot;.

## Profilnivåer {#profile-levels}

Adobe Marketo Engage prenumerationer på Adobe Identity Management System stöder olika profiler. Följande typer av användarprofiler är relevanta för den här integreringen.

<table>
 <tr>
  <td><strong>Adobe Admin Console systemadministratör</strong></td>
  <td>Ansvarig för att skapa identitetskoncept för Adobe och Marketo Engage i Adobe Admin Console. Tilldelad roll vid konfiguration av Adobe-organisationer.</td>
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
  <td><strong>Marketo Engage Admin</strong></td>
  <td>En person som har fått åtkomst till Marketo Engage med administratörsbehörighet. Beviljad roll i Marketo Engage, inte Adobe Admin Console (visas bara som"Admin" i <b>Redigera användare</b> modal).</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage-användare</strong></td>
  <td>En person som har fått tillgång till Marketo Engage. Inga administrativa behörigheter.</td>
 </tr>
</table>

## Vanliga frågor och svar {#faq}

Vanliga frågor [finns här](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Administratörsinställningar](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Lägg till eller ta bort en produktadministratör](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Lägg till eller ta bort en användare](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
