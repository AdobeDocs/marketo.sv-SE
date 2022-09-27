---
unique-page-id: 2360354
description: Lägg till Munchkin-spårningskod på din webbplats - Marketo Docs - produktdokumentation
title: Lägg till Munchkin-spårningskod på din webbplats
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
source-git-commit: dbb7478ac7b7e811bb9dfeb7c5e4a80ae400ab9b
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# Lägg till Munchkin-spårningskod på din webbplats {#add-munchkin-tracking-code-to-your-website}

Marketo anpassade JavaScript-spårningskod, som kallas Munchkin, spårar alla personer som besöker er webbplats så att ni kan reagera på besöken med automatiserade marknadsföringskampanjer. Även anonyma besökare spåras tillsammans med sina IP-adresser och annan information. **Utan den här spårningskoden kan du inte spåra besök eller annan aktivitet på din webbplats**!

>[!PREREQUISITES]
>
>Kontrollera att du har tillgång till en erfaren JavaScript-utvecklare. Marketo tekniska support är inte konfigurerad för att hjälpa till med felsökning av anpassad JavaScript.

## Lägg till spårningskod på din webbplats {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud-kunder kan också använda Marketo integrering i Adobe Launch för att inkludera Munchkin-skript på sina webbsidor. Skaffa appen [här](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Gå till **Administratör** område.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Klicka **Munchkin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Välj Asynkron för spårningskodtyp.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >I nästan alla fall bör du använda den asynkrona koden. [Läs mer](#types-of-munchkin-tracking-codes).

1. Klicka på och kopiera den Javascript-spårningskod som du vill använda på webbplatsen.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >Använd inte koden som visas på skärmbilden - du måste använda den unika koden som visas på ditt konto!

   >[!TIP]
   >
   >Lägg in spårningskod på de webbsidor du vill spåra. Det kan vara varje sida för mindre webbplatser, eller bara nyckelsidor på webbplatser som har många dynamiskt genererade webbsidor, användarforum och så vidare.

   För bästa resultat bör du använda den asynkrona Munchkin-koden och placera den inuti `<head>` element på sidorna. Om du använder den enkla koden (rekommenderas inte) är detta precis före `</body>` -tagg.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >För webbplatser med stor trafik (dvs. hundratusentals besök per månad) rekommenderar vi att du inte spårar anonyma personer. [Läs mer](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Lägg till spårningskod när flera arbetsytor används {#add-tracking-code-when-using-multiple-workspaces}

Om du använder Arbetsytor i ditt Marketo-konto har du förmodligen också separata webblänkar som motsvarar dina arbetsytor. I så fall kan du använda Munchkin tracking Javascript för att tilldela anonyma personer till rätt arbetsyta och partition.

1. Gå till **Administratör** område.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Klicka **Munchkin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Välj lämplig arbetsyta för de webbsidor som du vill spåra.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Om du inte använder den speciella arbetsytan Munchkin-koden tilldelas personerna standardpartitionen som skapades när ditt konto konfigurerades. Det heter till att börja med&quot;Standard&quot;, men du kan ha ändrat det på ditt Marketo-konto.

1. Välj **Asynkron** för spårningskodtyp.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Klicka på och kopiera den JavaScript-spårningskod som du vill använda på webbplatsen.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >Använd inte koden som visas på skärmbilden - du måste använda den unika koden som visas på ditt konto!

1. Placera spårningskoden på dina webbsidor i dialogrutan `<head>` -element. Nya personer som besöker den här sidan tilldelas den här partitionen.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Du kan bara använda ett Munchkin-spårningsskript för en enda partition och arbetsyta på en sida. Ta inte med spårningsskript för flera partitioner/arbetsytor på webbplatsen.

   >[!NOTE]
   >
   >Landningssidor som skapats i Marketo innehåller automatiskt spårningskod, så du behöver inte placera den här koden på dem.

## Typer av Munchkin-spårningskoder {#types-of-munchkin-tracking-codes}

Det finns tre typer av Munchkin-spårningskoder som du kan välja mellan. Alla effekter påverkar webbsidans laddningstid på olika sätt.

1. **Enkel**: har minst antal kodrader, men optimerar inte för webbsidans inläsningstid. Den här koden läser in jQuery-biblioteket varje gång en webbsida läses in.
1. **Asynkron**: minskar inläsningstiden för webbsidor.
1. **Asynkron jQuery**: minskar inläsningstiden för webbsidor och förbättrar också systemprestanda. Den här koden förutsätter att du redan har jQuery och inte kontrollerar att den har lästs in.

## Testa om din Munchkin-kod fungerar {#test-if-your-munchkin-code-is-working}

Så här kontrollerar du att din Munchkin-kod fungerar när du har lagt till den:

1. Besök webbsidan.

1. I My Marketo klickar du på **Analyser** platta.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Klicka **Webbsidesaktivitet**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Klicka på **Inställningar** flik, dubbelklicka **Aktivitetskälla**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Ändra aktivitetskällan till **Anonyma besökare (inklusive internetleverantörer)** och klicka **Använd**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Klicka på **Rapport** -fliken.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Om du inte ser några data väntar du några minuter och klickar sedan på uppdateringsikonen längst ned.
