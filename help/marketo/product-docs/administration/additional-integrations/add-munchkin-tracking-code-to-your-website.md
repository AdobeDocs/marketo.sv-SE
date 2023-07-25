---
unique-page-id: 2360354
description: "Lägg till [!DNL Munchkin] Spåra kod på din webbplats - Marketo Docs - produktdokumentation"
title: "Lägg till [!DNL Munchkin] Spåra kod på din webbplats"
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Lägg till [!DNL Munchkin] Spåra kod på din webbplats {#add-munchkin-tracking-code-to-your-website}

Marketo egen JavaScript-spårningskod, kallad [!DNL Munchkin], spårar alla personer som besöker er webbplats så att ni kan reagera på besöken med automatiserade marknadsföringskampanjer. Även anonyma besökare spåras tillsammans med sina IP-adresser och annan information. **Utan den här spårningskoden kan du inte spåra besök eller annan aktivitet på din webbplats**!

>[!PREREQUISITES]
>
>Kontrollera att du har tillgång till en erfaren JavaScript-utvecklare. Marketo tekniska support är inte konfigurerad för att hjälpa till med felsökning av anpassad JavaScript.

## Lägg till spårningskod på din webbplats {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud-kunder kan också använda Marketo integrering i Adobe Launch för att inkludera [!DNL Munchkin] skript på deras webbsidor. Skaffa appen [här](https://www.adobeexchange.com/experiencecloud.details.101054.html){target="_blank"}.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Klicka på **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Välj **[!UICONTROL Asynchronous]** for **[!UICONTROL Tracking Code Type]**.

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

   För bästa resultat bör du använda den asynkrona [!DNL Munchkin] och placera den inuti `<head>` element på sidorna. Om du använder den enkla koden (rekommenderas inte) är detta precis före `</body>` -tagg.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >För webbplatser med stor trafik (dvs. hundratusentals besök per månad) rekommenderar vi att du inte spårar anonyma personer. [Läs mer](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Lägg till spårningskod när flera arbetsytor används {#add-tracking-code-when-using-multiple-workspaces}

Om du använder Arbetsytor i ditt Marketo-konto har du förmodligen också separata webblänkar som motsvarar dina arbetsytor. I så fall kan du använda [!DNL Munchkin] spåra Javascript för att tilldela anonyma personer till rätt arbetsyta och partition.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Klicka på **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Välj lämplig arbetsyta för de webbsidor som du vill spåra.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Om du inte använder den speciella arbetsytan [!DNL Munchkin] koden tilldelas personerna standardpartitionen som skapades när ditt konto konfigurerades. Den heter &quot;[!UICONTROL Default]&quot; först, men du kan ha ändrat det på ditt eget Marketo-konto.

1. Välj **[!UICONTROL Asynchronous]** for **[!UICONTROL Tracking Code Type]**.

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
   >Du kan bara använda en [!DNL Munchkin] spårningsskript för en enskild partition och arbetsyta på en sida. Ta inte med spårningsskript för flera partitioner/arbetsytor på webbplatsen.

   >[!NOTE]
   >
   >Landningssidor som skapats i Marketo innehåller automatiskt spårningskod, så du behöver inte placera den här koden på dem.

## Typer av [!DNL Munchkin] Spårningskoder {#types-of-munchkin-tracking-codes}

Det finns tre typer av [!DNL Munchkin] spårningskoder som du kan välja mellan. Alla effekter påverkar webbsidans laddningstid på olika sätt.

1. **[!UICONTROL Simple]**: har minst antal kodrader, men optimerar inte för webbsidans inläsningstid. Den här koden läser in jQuery-biblioteket varje gång en webbsida läses in.
1. **[!UICONTROL Asynchronous]**: minskar inläsningstiden för webbsidor.
1. **[!UICONTROL Asynchronous jQuery]**: minskar inläsningstiden för webbsidor och förbättrar också systemprestanda. Den här koden förutsätter att du redan har jQuery och inte kontrollerar att den har lästs in.

## Testa om din [!DNL Munchkin] Koden fungerar {#test-if-your-munchkin-code-is-working}

För att kontrollera [!DNL Munchkin] koden fungerar när du har lagt till den:

1. Besök webbsidan.

1. I [!DNL My Marketo]klickar du på **[!UICONTROL Analytics]** platta.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Klicka på **[!UICONTROL Web Page Activity]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Klicka på **[!UICONTROL Setup]** flik, dubbelklicka **[!UICONTROL Activity Source]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Ändra [!UICONTROL Activity Source] till **[!UICONTROL Anonymous Visitors (including ISPs)]** och klicka **[!UICONTROL Apply]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Klicka på **[!UICONTROL Report]** -fliken.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Om du inte ser några data väntar du några minuter och klickar sedan på uppdateringsikonen längst ned.
