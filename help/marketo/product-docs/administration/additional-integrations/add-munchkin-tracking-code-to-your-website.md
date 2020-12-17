---
unique-page-id: 2360354
description: Lägg till Munchkin-spårningskod på din webbplats - Marketo Docs - Produktdokumentation
title: Lägg till Munchkin-spårningskod på din webbplats
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---


# Lägg till Munchkin-spårningskod på din webbplats {#add-munchkin-tracking-code-to-your-website}

Marketos skräddarsydda JavaScript-spårningskod, som kallas Munchkin, spårar alla personer som besöker er webbplats så att ni kan reagera på deras besök med automatiserade marknadsföringskampanjer. Även anonyma besökare spåras tillsammans med sina IP-adresser och annan information. ** Utan den här spårningskoden kan du inte spåra besök eller annan aktivitet på din webbplats!**

>[!PREREQUISITES]
>
>Kontrollera att du har tillgång till en erfaren JavaScript-utvecklare. Marketo Technical Support har inte konfigurerats för att hjälpa till med felsökning av anpassad JavaScript.

## Lägg till spårningskod på din webbplats {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud-kunder kan också använda Marketos integrering i Adobe Launch för att inkludera Munchkin-skript på sina webbsidor. Hämta appen [här](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Gå till **Admin** och klicka på **Munchkin** i trädet till vänster.

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   Välj Asynkron för spårningskodtyp.

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >I nästan alla fall bör du använda den asynkrona koden. [Läs mer.](#types-of-munchkin-tracking-codes)

   Klicka på och kopiera den Javascript-spårningskod som du vill använda på webbplatsen.

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >Använd inte koden som visas på skärmbilden - du måste använda den unika koden som visas på ditt konto!

   >[!TIP]
   >
   >Lägg in spårningskod på de webbsidor du vill spåra. Det kan vara varje sida för mindre webbplatser, eller bara nyckelsidor på webbplatser som har många dynamiskt genererade webbsidor, användarforum och så vidare.

   För bästa resultat bör du använda den asynkrona Munchkin-koden och placera den inuti `<head>`-elementen på sidorna. Om du använder den enkla koden (rekommenderas inte) är detta precis före taggen `</body>`.
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>För webbplatser med stor trafik (dvs. hundratusentals besök per månad) rekommenderar vi att du inte spårar anonyma personer. [Läs mer.](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/)

## Lägg till spårningskod när flera arbetsytor används {#add-tracking-code-when-using-multiple-workspaces}

Om du använder Arbetsytor i ditt Marketo-konto har du förmodligen också separata webblänkar som motsvarar dina arbetsytor. I så fall kan du använda Munchkin tracking Javascript för att tilldela anonyma personer till rätt arbetsyta och partition.

1. Gå till Admin och klicka på Munchkin i trädet till vänster.

![](assets/image2015-8-25-16-3a28-3a41.png)

1. Välj lämplig arbetsyta för de webbsidor som du vill spåra.

![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>Om du inte använder den speciella arbetsytan Munchkin-koden tilldelas personerna standardpartitionen som skapades när ditt konto konfigurerades. Det heter till att börja med&quot;Standard&quot;, men du kan ha ändrat det i ditt eget Marketo-konto.

1. Välj Asynkron för spårningskodtyp.

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. Klicka på och kopiera den JavaScript-spårningskod som du vill använda på webbplatsen.

![](assets/image2015-8-25-16-3a34-3a7.png)

>[!CAUTION]
>
>Använd inte koden som visas på skärmbilden - du måste använda den unika koden som visas på ditt konto!

1. Placera spårningskoden på dina webbsidor i `<head>`-elementet. Nya personer som besöker den här sidan tilldelas den här partitionen.

![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>Du kan bara använda ett Munchkin-spårningsskript för en enda partition och arbetsyta på en sida. Ta inte med spårningsskript för flera partitioner/arbetsytor på webbplatsen.

>[!NOTE]
>
>Landningssidor som skapats i Marketo innehåller automatiskt spårningskod, så du behöver inte placera den här koden på dem.

## Typer av Munchkin-spårningskoder {#types-of-munchkin-tracking-codes}

Det finns tre typer av Munchkin-spårningskoder som du kan välja mellan. Alla effekter påverkar webbsidans laddningstid på olika sätt.

1. **Enkelt**: har minst antal kodrader, men optimerar inte för webbsidans inläsningstid. Den här koden läser in jQuery-biblioteket varje gång en webbsida läses in.
1. **Asynkron**: minskar inläsningstiden för webbsidor.
1. **Asynkron jQuery**: minskar inläsningstiden för webbsidor och förbättrar också systemprestanda. Den här koden förutsätter att du redan har jQuery och inte kontrollerar att den har lästs in.

## Testa om din Munchkin-kod fungerar {#test-if-your-munchkin-code-is-working}

Så här kontrollerar du att din Munchkin-kod fungerar när du har lagt till den:

1. Besök webbsidan.
1. Gå till **Analytics**.

   ![](assets/mainnav-analytics-hand.png)

1. Klicka på **Webbsidesaktivitet**.

   ![](assets/webanalytics.png)

1. Klicka på fliken **Inställningar**, dubbelklicka på **Aktivitetskälla** och ändra den till **Anonyma besökare (inklusive Internet-leverantörer)**.

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. Klicka på fliken **Rapport**. Om du inte ser några data väntar du några minuter och klickar sedan på uppdateringsikonen längst ned.

