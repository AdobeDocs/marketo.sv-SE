---
unique-page-id: 11383945
description: Understanding Facebook Offline Conversions - Marketo Docs - Product Documentation
title: Förstå offlinekonverteringar för Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Förstå konverteringar offline för [!DNL Facebook] {#understanding-facebook-offline-conversions}

Leadannonskampanjer på Facebook genererar leads och skickar dem till Marketo för användning i marknadsföringskampanjer. Utan synlighet i offlinekonverteringar kan annonseraren [!DNL Facebook] inte veta vilka annonser som är mest effektiva. Här är ett exempel.

>[!NOTE]
>
>**Exempel**
>
>[!UICONTROL Facebook Lead Ads] kör tre annonser.
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
>Utan offlinekonverteringar skulle annonsören förmodligen investera mer i annons 3. Med konverteringsdata offline kommer annonsören mer sannolikt att investera i annons 1.

Du kan [konfigurera offlinekonverteringar för Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) för att skicka offlineannonsprestanda till [!DNL Facebook].

1. Kontrollera att [[!DNL Facebook] [!UICONTROL LaunchPoint]-integreringen &#x200B;](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) är uppdaterad.
1. Mappa faser i din intäktscykelmodell till offlinekonverteringsfaser på [!DNL Facebook].
1. När en [!DNL Facebook]-lead genereras från en [!DNL Facebook]-lead-annons och når en mappad fas skickar Marketo tillbaka offlinekonverteringsdata till [!DNL Facebook] flera gånger dagligen via ett säkert, automatiserat API. Data visas i rapporten [!DNL Facebook] Ads Manager.

>[!MORELIKETHIS]
>
>[Konfigurera [!DNL Facebook] offlinekonverteringar](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
