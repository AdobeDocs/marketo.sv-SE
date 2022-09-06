---
unique-page-id: 10099077
description: E-postleverans Power Pack - Så här importerar du en SeedList - Marketo Docs - Produktdokumentation
title: E-postleverans, Power Pack - Så här importerar du en Seedlist
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
source-git-commit: 4448d6e082c0c4fad35fc2980446175bffe47e4b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Power Pack för e-postleverans: Importera en lista {#email-deliverability-power-pack-how-to-import-a-seedlist}

En startvärdeslista är en lista över e-postkonton hos flera postlådeleverantörer, inklusive Google Apps, Hotmail, Yahoo!, osv., som används för att beräkna hur snabbt inkorg- och skräppostmappen levereras. Så här hämtar du listan till din Marketo-instans.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

## Importera en utskickslista {#import-a-seedlist}

1. I My Marketo väljer du **Leveransverktyg**.

   ![](assets/email-deliverability-power-pack-1.png)

1. Klicka **Inkorgsinformant**.

   ![](assets/two-1.png)

1. Klicka **Hämta SeedList**.

   ![](assets/three-1.png)

1. Klicka **Exportera lista**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Välj **Optimera lista** om du vill att 250ok ska [optimera listan](https://help.returnpath.com/hc/en-us/articles/360046746451-What-is-250ok-s-seedlist-optimizer-and-why-should-I-use-it-) för dig. Välj **Anpassa lista** om du vill markera de seedlisteområden som du vill ta med.

1. Efter exporten visas listan som en TXT-fil i webbläsarens nedladdningsmapp. Hämta den och [import](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) i din Marketo-instans som en statisk lista.

   ![](assets/five.png)

   >[!TIP]
   >
   >Ge listan ett namn som gör det enkelt att hitta.

   >[!CAUTION]
   >
   >Du får ett begränsat antal av dessa Inbox Informant-kampanjer per månad. Om du vill se hur många du får kan du titta i din 250ok **Kontoinställningar**. Kontakta din Marketo-säljare om du vill ha mer information.

## Hämtar nya dirigeringslistor {#acquiring-new-seedlists}

Din sändlista kan ändras så ofta som varje månad. Det är viktigt att du regelbundet loggar in på Power Pack för e-postleverans och kontrollerar statusen för din startlista. När nya adresser läggs till eller en uppdatering krävs på din sida får du en varning via gränssnittet på sidan Hämta seedlist.

När den statiska listan i Marketo har skapats kan du börja skicka till den för att testa e-postens placering i inkorgen.
