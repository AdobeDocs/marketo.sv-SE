---
description: Konfigurera MSI-vyer - Marketo Docs - produktdokumentation
title: Konfigurera MSI-vyer
hide: true
hidefromtoc: true
source-git-commit: f4930d1747f1ca893d7494afc3dcbeb8c6398e93
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Konfigurera MSI-vyer {#setting-up-msi-views}

När du installerar plugin-programmet Sales Insight i Dynamics läggs de bästa valen och tillhörande instrumentpaneler automatiskt till på webbplatskartan. Om kontrollpanelerna av någon anledning inte läggs till gör du så här för att lägga till dem manuellt.

1. Klicka på kugghjulsikonen i Dynamics och välj **Avancerade inställningar** i listrutan.

1. Klicka på längst upp till vänster på skärmen **Inställningar**. Välj Anpassningar under Anpassning.

1. Klicka **Anpassa systemet**.

1. Klicka i trädet till vänster på **Klienttillägg** och dubbelklicka **Webbplatskarta**.

1. Klicka på högerpilen för att gå till nästa sida. Under Försäljning hittar du Marketo. Om du inte gör det kontrollerar du att du har importerat paketet korrekt.

   >[!NOTE]
   >
   >Under Marketo bör du ha: Bästa val, Min e-post, Webbaktivitet och anonym webbaktivitet. Om någon av dessa instrumentpaneler saknas klickar du på plustecknet ovanför Försäljning och lägger till dem som ett delområde.

1. Klicka på en kontrollpanel för att markera den. I kolumnen till höger anger du respektive information nedan för var och en av dem. Du kan ignorera alla kategorier som inte finns med i listan.

   **Bästa val**</br>
URL: MainviewBestbets.html</br>
Ikon: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Titel: Bästa val

   **Min e-postadress**</br>
URL: mkt_/MainViewMyEmail.html</br>
Ikon: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
Titel: Min e-postadress

   **Webbaktivitet**</br>
URL: mkt_/MainViewWebActivity.html</br>
Ikon: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Titel: Webbaktivitet

   **Anonym webbaktivitet**</br>
URL: mkt_/MainViewWebActivity.html</br>
Ikon: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Titel: Anonym webbaktivitet

1. Klicka **Spara** när det är klart.
