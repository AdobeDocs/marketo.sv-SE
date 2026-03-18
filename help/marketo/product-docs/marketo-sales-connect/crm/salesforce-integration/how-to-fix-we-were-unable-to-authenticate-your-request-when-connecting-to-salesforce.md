---
unique-page-id: 14352484
description: Få hjälp med att åtgärda felet Det gick inte att autentisera din begäran vid anslutning av Sales Connect till Salesforce. Felsök autentiseringsproblem.
title: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 3%

---

# Så här åtgärdar du&quot;Det gick inte att autentisera din begäran&quot; vid anslutning till [!DNL Salesforce] {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du får felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; när du försöker ansluta [!DNL Sales Connect] till [!DNL Salesforce] kan det finnas en begränsning för din åtkomst till API:t för [!DNL Salesforce]. Kontrollera med din [!DNL Salesforce]-administratör att följande saker finns på plats.

## Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en [!DNL Salesforce]-administratör logga in på SFDC.
1. Välj **[!UICONTROL Setup]**.
1. Välj **[!UICONTROL Manage Users]**.
1. Välj **[!UICONTROL Profiles]**.
1. Hitta den profil som ToutApp-användarna befinner sig under och klicka på **[!UICONTROL Edit]**.
1. Bläddra ned till **[!UICONTROL Administrative Permissions]** och kontrollera att **[!UICONTROL API Enabled]** är markerat.

## Kontrollera om [!DNL Salesforce] blockerar [!DNL Sales Connect] från anslutning {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Låt en [!DNL Salesforce]-administratör logga in på SFDC.
1. Välj **[!UICONTROL Setup]**.
1. Välj **[!UICONTROL Manage Apps]**.
1. Välj **[!UICONTROL Connected Apps OAuth Usage]**.
1. Se till att [!DNL Sales Connect] visar [!UICONTROL Block] bredvid den. Om [!UICONTROL Unblock] visas klickar du på knappen för att häva blockeringen av [!DNL Sales Connect] för åtkomst till [!DNL Salesforce].
