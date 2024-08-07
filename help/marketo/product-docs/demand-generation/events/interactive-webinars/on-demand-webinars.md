---
description: On Demand Webinars - Marketo Docs - produktdokumentation
title: On-Demand-webbinarier
feature: Interactive Webinars
exl-id: 65bfc1d2-6382-4cfa-9560-69cbb0c37c42
source-git-commit: 7de0aed6be29a304276f2b3f96dd60974b4c4eb6
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# On-Demand-webbinarier {#on-demand-webinars}

On-Demand Webinars fångar och förfinar leads som registrerats för ditt event och inte deltog, men vill få information om evenemanget genom att titta på inspelningen. Information som Namn, E-post-ID och Bevakningsdatum/varaktighet kan hämtas i Marketo Engage och användas som mål för de här no-show-leads.

URL:en för webbinariet Joining som delades med de registrerade före evenemanget kan användas för att titta på inspelningen on demand. När en registrant som inte deltog i live-evenemanget (t.ex. en lead med programstatus som &quot;No-Show&quot;) klickar på webbinariets anslutnings-URL, ändras leadets programstatus från &quot;No-Show&quot; till &quot;Attended On-Demand&quot;. Programstatusen för de leads som tittade på händelsen live och har statusen &quot;Attended&quot; påverkas inte om de bestämmer sig för att besöka URL:en Joining och titta på inspelningen on demand.

Adobe Connect, den teknik som driver Interactive Webinars, håller reda på besökets längd liksom hur länge ledtrådarna som tittar på inspelningen ska vara och rapporterar informationen till Marketo Engage dagligen. Spårning för On-Demand-webbinarier stoppas 30 dagar efter händelsen. Längden kan inte ändras.

Marketo Engage tillhandahåller bevakningsstatistik för On Demand-webbinarier på fliken Dashboard med hjälp av följande widgetar:

* On-Demand Summary: Detta ger en sammanfattning av antalet besökare (no-Shows) som tittar på inspelningen efter händelsen på en viss dag(ar)

* Statistik på begäran: Den här widgeten innehåller information om:
   * Dagar inspelningen finns tillgänglig för visning - Hjälper marknadsförare att utföra åtgärder, som att köra e-postkampanjer nära slutet av tillgänglighetsperioden på 30 dagar.
   * Det totala antalet besökare för webbinarier på begäran hittills - antalet alla registranter som inte har kunnat se on-demand-inspelningen hittills.
   * Genomsnittlig bevakningstid i minuter för alla besökare - Ger marknadsförarna en uppfattning om hur mycket av inspelningen som visas och vad Smart Campaigns kan användas för att rikta leads över en viss bevakningstid.

![](assets/on-demand-webinars-1.png)

>[!NOTE]
>
>Vyer räknas bara när bevakningstiden överskrider en minut.

Filtren och utlösarna för interaktiva webbinarier har ändrats för att passa On-Demand Webinars. Utlösaren&quot;Attends Event&quot; och filtret&quot;Has Attention event&quot; läggs till med en extra begränsning (&quot;Event Mode&quot;), där en marknadsförare kan välja om målet är Live-målgrupp eller On-Demand-målgrupp. Om villkoret Händelseläge inte är markerat används både Live-målgruppen och On-Demand-målgruppen. Andra begränsningar, t.ex. &quot;Bevakningsdatum&quot; och &quot;Bevakningstid&quot;, kan användas med händelseläget &quot;On-Demand&quot;. Inaktivitetsfiltret &quot;Har inte deltagit i en händelse&quot; kan även användas för webbinarier på begäran i händelseläget &quot;On-Demand&quot;.
