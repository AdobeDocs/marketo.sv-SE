---
unique-page-id: 11383945
description: Understanding Facebook Offline Conversions - Marketo Docs - produktdokumentation
title: Förstå offlinekonverteringar för Facebook
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Om offlinekonverteringar för Facebook {#understanding-facebook-offline-conversions}

Leadannonskampanjer på Facebook genererar leads och skickar dem till Marketo för användning i marknadsföringskampanjer. Utan synlighet i offlinekonverteringar kan annonsören på Facebook inte veta vilka annonser som är mest effektiva. Här är ett exempel.

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
>
Baserat på enbart dessa siffror verkar Ad 3 vara den mest effektiva.
>
>Men när man tittar på data på Marketo-sidan utvecklas en annan historia.
>
>* Annons 1 genererar 10 försäljningar
>* Annons 3 genererar 2 försäljningar

>
>
Det innebär att annonsering 1, trots att den genererade färre leads, hade 50 procents framgång, medan annons 3 nästan inte alls var effektiv.
>
>Utan offlinekonverteringar skulle annonsören förmodligen investera mer i annons 3. Med offlinekonverteringsdata är det troligare att annonsören investerar i annons 1.

Du kan [konfigurera offlinekonverteringar för Facebook](set-up-facebook-offline-conversions.md) för att skicka offlineannonsprestanda till Facebook.

1. Se till att din [LaunchPoint-integrering på Facebook](../../../product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) är aktuell.
1. Mappa faser i intäktscykelmodellen till offlinekonverteringsfaser på Facebook.
1. När en Facebook-lead genereras från en Facebook-annons och når en mappad scen skickar Marketo tillbaka konverteringsdata till Facebook flera gånger dagligen via ett säkert, automatiserat API. Informationen visas i Facebook Ads Manager-rapporten.

>[!MORELIKETHIS]
>
>* [Konfigurera offlinekonverteringar för Facebook](set-up-facebook-offline-conversions.md)

>



