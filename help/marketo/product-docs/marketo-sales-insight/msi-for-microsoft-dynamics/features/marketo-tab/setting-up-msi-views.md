---
description: Konfigurera MSI-vyer - Marketo Docs - produktdokumentation
title: Konfigurera MSI-vyer
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Konfigurera MSI-vyer {#setting-up-msi-views}

Om du installerar plugin-programmet [!DNL Sales Insight] i Dynamics läggs [!DNL Best Bets] och relaterade instrumentpaneler automatiskt till på webbplatskartan. Om kontrollpanelerna av någon anledning inte läggs till gör du så här för att lägga till dem manuellt.

1. Klicka på kugghjulsikonen i Dynamics och välj **[!UICONTROL Advanced Settings]** i listrutan.

1. Klicka på **[!UICONTROL Settings]** i skärmens övre vänstra hörn. Välj **[!UICONTROL Customizations]** under Anpassning.

1. Klicka på **[!UICONTROL Customize the System]**.

1. Klicka på **[!UICONTROL Client Extensions]** i trädet till vänster och dubbelklicka på **[!UICONTROL Site Map]**.

1. Klicka på högerpilen för att gå till nästa sida. Under Försäljning hittar du Marketo. Om du inte gör det måste du kontrollera att du har importerat paketet korrekt.

   >[!NOTE]
   >
   >Under Marketo bör du ha: Bästa val, Min e-post, Webbaktivitet och anonym webbaktivitet. Om någon av dessa instrumentpaneler saknas klickar du på plustecknet ovanför Försäljning och lägger till dem som ett delområde.

1. Klicka på en kontrollpanel för att markera den. I kolumnen till höger anger du respektive information nedan för var och en. Du kan ignorera alla kategorier som inte finns med i listan.

   **Bästa val**</br>
URL: MainviewBestbets.html</br>
Ikon: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Titel: Bästa val

   **Min e-postadress**</br>
URL: mkt_/MainViewMyEmail.html</br>
Ikon: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail </br>
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

1. Klicka på **[!UICONTROL Save]** när du är klar.
