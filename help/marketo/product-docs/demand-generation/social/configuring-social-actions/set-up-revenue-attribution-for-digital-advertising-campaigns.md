---
unique-page-id: 10098812
description: Ställ in intäktsattribuering för digitala Advertising-kampanjer - Marketo Docs - produktdokumentation
title: Ställ in intäktsattribuering för digitala Advertising-kampanjer
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Ställ in intäktsattribuering för digitala Advertising-kampanjer {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Så här skapar du intäktsattribuering för digitala annonskanaler och kampanjer. När ni har skapat det kan ni attribuera intäkter från första beröringen och multitouch för digitala annonser på samma sätt som i andra Marketo-program.

>[!IMPORTANT]
>
>Den 31 juli 2024 började vi ta bort den här funktionen. Du kommer inte att kunna skapa nya resurser. Befintliga tillgångar kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

När du har konfigurerat ditt första annonseringsprogram i Marketo kan du klona och uppdatera det för andra kanaler. Du kan till exempel klona ett LinkedIn-program till ett Facebook.

Med separata program kan ni sedan spåra antalet konverteringar från var och en och se era program i Program Analyzer, Opportunity Influence Analyzer och andra Marketo Analytics-funktioner.

>[!PREREQUISITES]
>
>* Konfigurera en kanaltagg med statusvärden och programframgångar (till exempel Digital Advertising eller Social Paid och PPC)
>* Skapa eller redigera ett formulär för att skicka en frågesträng via personen
>* Se till att ni har tillgång till vissa funktioner i IntäktsCycle Analytics för att rapportera om era annonskanaler och kampanjer

## Skapa ett standardprogram {#create-a-default-program}

Till skillnad från vissa program (till exempel e-post) som kan köras regelbundet under en viss tidsperiod, är standardprogram alltid aktiverade.

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-5.png)

1. Klicka på **Nytt** och välj **Nytt program**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Om du redan har ett program på plats kan du [klona det](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >När du klonar ett program måste du se till att ersätta namnen i frågesträngsfälten i de smarta listorna.

1. Placera det nya programmet i en viss kampanjmapp när det första programmet har angetts.

   >[!NOTE]
   >
   >**Exempel**
   >
   >En frågesträng som skickas via webbadressen hjälper Marketo att veta vilken annonskampanj någon klickade på när de blev en person i Marketo.
   >
   >Du kan skapa en frågesträngsmetod som innehåller alla variabler som du vill mäta. Marketo använder dessa variabler för att lägga till personer i dina olika program.
   >
   >Du kan till exempel använda kanaltypen Kanal_Kanal_Resurs_Region. Det kan se ut så här: SP_FB_NewGuide_US. **Obs!**: förkortningar sparar utrymme.
   >
   >Du kan också ange det som Channel_Adsource_AssetName_Region_UniqueIdNumber. Det kan se ut så här: Social-Paid_Facebook_NewGuide_NA_123.

## Skapa en smart kampanj för nya namn {#create-a-smart-campaign-for-new-names}

1. I den smarta kampanjen skapar du en smart lista som innehåller två utlösare och två filter, som visas.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >Frågesträngen som används i de två utlösarna och filtret **Program som har hämtat namn** är unik för dig. Frågesträngarna som visas här är till exempel bara. Om du klonade fältet ersätter du dessa fält.

1. Skapa ett flödessteg om du vill ändra attributet till **förvärvsprogram** och ange det nya värdet till det värde som du har definierat för betalda sociala kampanjer.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Schemalägg och aktivera kampanjen.

## Skapa en smart kampanj för status/lyckat program {#create-a-smart-campaign-for-status-program-success}

Ni behöver en andra smart kampanj för att ändra personernas status, så att de kan uppnå programframgångar och inkluderas i intäktsattribueringsberäkningarna.

1. I utlösaren **Fyller i formulär** anger du programnamnet i frågesträngen. Om du klonar programmet ersätter du bara det gamla frågesträngnamnet med det nya.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Skapa flödessteg för att ändra status till en som är kopplad till programslutförande.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >I exemplet ovan visas **Konverterad**, men det beror på dina status-/framgångsvärden.

1. Schemalägg och aktivera kampanjen.

## Skapa din annons {#create-your-ad}

Skapa den nya annonsen när du har konfigurerat programmet och kampanjerna.

1. Gå till kanalen, till exempel LinkedIn eller Facebook.
1. Skapa en ny annons.
1. Välj en Marketo-landningssida som mål för Call To Action i kampanjen.
1. Lägg till frågesträngen i URL:en.

   >[!NOTE]
   >
   >**Exempel**
   >
   >Så här kan du lägga till all information som du har angett i en faktisk URL-adress. Objekten avgränsas med ett et-tecken (&amp;):
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** är den person-Source som används som kanalidentifierare
   >* **comment** är den unika identifieraren som skapats för varje program
   >* **läger** är kampanjen i Facebook, LinkedIn eller Google
   >* **k** är nyckelordet eller resursnamnet som du vill hämta
   >
   >**De här fyra termerna måste bestå av gemener och det får inte finnas några blanksteg i URL:en för att informationen ska kunna hämtas.**

## Bästa praxis {#best-practices}

Använd en enda kanaltagg för att representera alla digitala Advertising, eller använd flera kanaltaggar om du vill ha mer detaljerade jämförelser med dina andra marknadsföringskanaler (till exempel Socialbetald, Sökbetald, Visning, Återmarknadsföring).

Skapa sedan olika program för varje rapportvy du behöver. Använd ett gemensamt ID som parameter i URL:en (till exempel BC) i frågesträngen om du har 10 regioner som startar en&quot;Big Campaign&quot; tillsammans och vill kunna visa resultat i olika regioner.

Om ni vill rapportera om varje region och de samlade resultaten av Big Campaign skapar ni 11 program - ett för varje region och ett för Big Campaign. Varje program refererar endast de relevanta tecknen från frågesträngen (till exempel BC).

Det finns avsiktlig överlappning mellan Big Campaign och regionsprogrammen, så du vill inte rapportera om det totala antalet människor i alla elva programmen, eftersom vissa finns både i Big Campaign och i ett av regionsprogrammen.
