---
unique-page-id: 10099077
description: E-postleverans Power Pack - Så här importerar du en Seedlist - Marketo Docs - Produktdokumentation
title: E-postleverans, Power Pack - Så här importerar du en Seedlist
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Power Pack för e-postleverans: Importera en Seedlist {#email-deliverability-power-pack-how-to-import-a-seedlist}

En startvärdeslista är en lista över e-postkonton hos flera postlådeproviders, bland annat Google Apps, Hotmail, Yahoo!, som används för att beräkna hur många inkorgar som kan levereras jämfört med skräppostmappar. Så här hämtar du listan till din Marketo-instans.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

## Importera en Seedlist {#import-a-seedlist}

1. Gå till **Leveransverktyg**.

   ![](assets/one-1.png)

1. Klicka på **Inkorgsinfo**.

   ![](assets/two-1.png)

1. Klicka på **Hämta Seedlist**.

   ![](assets/three-1.png)

1. Klicka på **Exportera lista**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Välj **Optimera lista** om du vill att 250ok ska [optimera listan](https://support.250ok.com/hc/en-us/articles/216763528-What-is-the-list-optimizer-and-why-should-I-use-it-) åt dig. Välj **Anpassa lista** om du vill välja de utseendelisteområden som du vill ta med.

1. Efter exporten visas listan som en TXT-fil i webbläsarens nedladdningsmapp. Hämta den och [importera](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) den till din Marketo-instans som en statisk lista.

   ![](assets/five.png)

   >[!TIP]
   >
   >Ge listan ett namn som gör det enkelt att hitta.

   >[!CAUTION]
   >
   >Du får ett begränsat antal av dessa Inbox Informant-kampanjer per månad. Om du vill se hur många du får kan du titta i dina 250ok **Kontoinställningar**. Kontakta er säljare på Marketo om du vill ha mer information.

## Hämtar nya dirigeringslistor {#acquiring-new-seedlists}

Din sändlista kan ändras så ofta som varje månad. Det är viktigt att du regelbundet loggar in på Power Pack för e-postleverans och kontrollerar statusen för din startlista. När nya adresser läggs till eller en uppdatering krävs på din sida får du en varning via gränssnittet på sidan Hämta seedlist.

När den statiska listan i Marketo har skapats kan du börja skicka till den för att testa e-postens placering i inkorgen.
