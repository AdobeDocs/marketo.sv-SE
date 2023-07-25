---
unique-page-id: 11383945
description: Understanding Facebook Offline Conversions - Marketo Docs - Product Documentation
title: Förstå Facebook offlinekonverteringar
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Förstå Facebook offlinekonverteringar {#understanding-facebook-offline-conversions}

Facebook Lead Ads-kampanjer genererar leads och skickar dem till Marketo för användning i marknadsföringskampanjer. Utan synlighet i offlinekonverteringar kan Facebook annonsörer dock inte veta vilka annonser som är mest effektiva. Här är ett exempel.

>[!NOTE]
>
>**Exempel**
>
>Facebook Lead Ads har tre annonser.
>
>* Annons 1 genererar 20 leads
>* Annons 2 genererar 30 leads
>* Annons 3 genererar 50 leads
>
>Baserat på enbart dessa siffror verkar Ad 3 vara den mest effektiva.
>
>Men när man tittar på data på Marketo-sidan utvecklas en annan historia.
>
>* Annons 1 genererar 10 försäljningar
>* Annons 3 genererar 2 försäljningar
>
>Det innebär att annonsering 1, trots att den genererade färre leads, hade 50 procents framgång, medan annons 3 nästan inte alls var effektiv.
>
>Utan offlinekonverteringar skulle annonsören förmodligen investera mer i annons 3. Med offlinekonverteringsdata är det troligare att annonsören investerar i annons 1.

Du kan [konfigurera offlinekonverteringar för Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) för att skicka annonsprestanda offline till Facebook.

1. Se till att [Integrering med facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) är uppdaterad.
1. Mappa faser i intäktscykelmodellen till offlinekonverteringsfaser i Facebook.
1. När en Facebook-lead genereras från en Facebook Lead Ad och når en mappad fas skickar Marketo tillbaka konverteringsdata till Facebook flera gånger dagligen via ett säkert, automatiserat API. Data visas i Facebook Ads Manager Report.

>[!MORELIKETHIS]
>
>[Konfigurera offlinekonverteringar för Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
