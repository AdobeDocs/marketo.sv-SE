---
description: On Demand Webinars - Marketo Docs - produktdokumentation
title: On-Demand-webbinarier
hide: true
hidefromtoc: true
feature: Interactive Webinars
source-git-commit: 49a75b6aef25787a68554dff3a847279ef8ba12a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# On-Demand-webbinarier {#on-demand-webinars}

On-Demand Webinars fångar och förfinar leads som registrerats för ditt event och inte deltog, men vill få information om evenemanget genom att titta på inspelningen. Information som Namn, E-post-ID och Bevakningsdatum/varaktighet kan hämtas i Marketo Engage och användas som mål för dessa no-show-leads.

Webbseminariets anslutnings-URL som delades med de registrerade före evenemanget kan användas som en länk för att se inspelningen on demand. När en registrant, som inte deltog i live-evenemanget, dvs. en lead med programstatus som &quot;No-Show&quot;, klickar på webbseminariets anslutnings-URL, ändras programstatusen för en sådan lead från &quot;No-Show&quot; till &quot;Attended On-Demand&quot;. Observera att programstatusen för leads som har tittat på händelsen live och har statusen &quot;Attended&quot; (Tillägen) inte påverkas även om de besöker webbadressen Joining (Gå med) och tittar på inspelningen on demand.

Adobe Connect, den teknik som ligger till grund för Interactive Webinars, håller reda på besöket samt hur länge de leads som har sett inspelningen har varat och rapporterar samma information om Marketo varje dag. Inspelningen är tillgänglig på Joining URL under 30 dagar efter händelsen och längden är fast.

Marketo tillhandahåller bevakningsstatistik för On Demand Webinars på fliken Dashboard med hjälp av följande två widgetar:
1. On-Demand Summary: Detta ger en dagvis sammanfattning av antalet besökare (no-Shows) som har tittat på inspelningen av evenemanget.
2. Statistik på begäran: Dessa widgetar ger information om: a. Dagar då inspelningen på begäran är tillgänglig för visning. Detta kan hjälpa marknadsförarna att vidta åtgärder som att köra e-postkampanjer närmare slutet av tillgänglighetsperioden för inspelning på 30 dagar.
b. Totalt antal besökare för webbinarier på begäran till dagens datum. Detta skulle vara antalet av alla registranter som inte har kunnat se på on-demand-inspelningen fram till datumet.
c. Genomsnittlig bevakningstid i minuter för alla besökare. Detta ger marknadsföraren en uppfattning om hur mycket av inspelningen som visas och vilka smarta kampanjer som kan användas för att rikta leads över en viss bevakningstid.

SCREENSHOT

Filtren och utlösarna för interaktiva webbinarier har ändrats för att passa On-Demand Webinars. Utlösaren&quot;Attends Event&quot; och filtret&quot;Has Attention event&quot; läggs till med en extra begränsning,&quot;Event Mode&quot;, där en marknadsförare kan välja om målet är Live-målgrupp eller On-Demand-målgrupp. Om villkoret Händelseläge inte är markerat så används både Live- och On-Demand-målgrupper. Andra begränsningar som &quot;Bevakningsdatum&quot; och &quot;Bevakningstid&quot; kan användas med &quot;On-Demand&quot;-händelseläget. Inaktivitetsfiltret &quot;Har inte deltagit i en händelse&quot; kan också användas för webbinarier på begäran i händelseläget &quot;On-Demand&quot;.
