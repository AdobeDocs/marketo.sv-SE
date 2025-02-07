---
title: Content Accelerator doc
description: Lär dig hur..
hide: true
hidefromtoc: true
source-git-commit: 87dfe8e1f3f10940a9079e22a056ccb4f5ea9a95
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Använda AI Assistant Content Accelerator {#use-the-ai-assistant-content-accelerator}

AI Assistant Content Accelerator är en funktion i Marketo Engage Email Designer som hjälper dig att skapa aktuella, högpresterande och intuitiva e-postmeddelanden på ett produktivt sätt. Detta uppnås genom Adobe generative AI-teknik och ett snabbt bibliotek tillsammans med Firefly för bildgenerering som hjälper till att skapa lämpligt innehåll för en viss individ/köpgrupp, marknadsföringsresa, kommunikationsstrategi, ton osv. Specifika varumärkesresurser kan också användas för att skapa innehåll.

>[!PREREQUISITES]
>
>AI Assistant Content Accelerator är inte aktiverat som standard. Du måste först godkänna villkoren för Core Gen-AI och de kompletterande villkoren för att använda Gen-AI-funktionen i e-postprogrammet för Designer. Kontakta kontoteamet (din kontoansvarige) för mer information.

Det finns tre primära användningsområden för AI Assistant Content Accelerator:

* [Skapa en ämnesrad](#create-a-subject-line) för ditt e-postmeddelande
* [Skapa innehåll för ett visst avsnitt](#create-content-for-a-specific-section) i e-postmeddelandet
* [Skapa ett helt e-postmeddelande](#create-an-entire-email) från en markerad mall

## Skapa en ämnesrad {#create-a-subject-line}

När ett e-postmeddelande skapas med Designer New Email anger du en tillfällig ämnesrad.

SCREENSHOT

När e-postmeddelandet har skapats finns ämnesraden i kolumnen _Detaljer_ till höger. Klicka på AI-assistentknappen ( ![Filterikon](assets/icon-ai-assistant.png) ) bredvid om du vill ha hjälp med att skapa en ny ämnesrad med Gen AI-funktionen.

SCREENSHOT

—STOPPAD REDIGERING HÄR—

Om du redan har använt en ämnesrad och vill använda den som referens för genereringen, växlar du till knappen &quot;Använd referensinnehåll&quot;.

Ange uppmaningen att anpassa ämnesraden. Ange relevanta textinställningar och överför alla varumärkesresurser som du vill använda som referens för att skapa en lämplig ämnesrad.

SCREENSHOT

Textinställningarna omfattar:

<table><tbody>
  <tr>
    <td><b>Buying Group</b></td>
    <td>Den specifika köpgrupp ni riktar in er på (t.ex. koncernchef, påverkare, beslutsfattare).</td>
  </tr>
  <tr>
    <td><b>Marknadsföringsresa</b></td>
    <td>Mottagare i ett visst stadium av marknadsföringsresan (t.ex. Discover, Evaluate, Commit).</td>
  </tr>
  <tr>
    <td><b>Kommunikationsstrategi</b></td>
    <td>Syftet med kommunikationen (t.ex. brådskande frågor, socialt bevis, information).</td>
  </tr>
  <tr>
    <td><b>Språk</b></td>
    <td>Det språk som du vill att ämnesraden ska skapas på.</td>
  </tr>
  <tr>
    <td><b>Ton</b></td>
    <td>Ton som du vill att innehållet ska genereras i (t.ex. Inspiration, Exciting, Humorous).</td>
  </tr>
  <tr>
    <td><b>Emojis</b></td>
    <td>Gör att uttryckssymboler kan inkluderas i det genererade innehållet.</td>
  </tr>
</tbody>
</table>

En exempelinställning för fylld text ser ut så här:

SCREENSHOT

Du kan också välja att överföra en varumärkesresurs för att använda innehåll i resursen som ett referensinnehåll för att skapa ämnesraden.

SCREENSHOT

När du har markerat en variant kan du välja att använda den genom att markera varianten i kryssrutan och klicka på Markera. Du kan också förfina den genom att klicka på Förfina och ändra inställningarna. Du kan också ge feedback genom reglage uppåt eller nedåt så att Gen-AI-tekniken förstår vad som fungerar enligt dina önskemål.

När du väljer kan du se hur ämnesraden fylls i i din e-postinformation

SCREENSHOT

## Skapa innehåll för ett visst avsnitt i e-postmeddelandet {#create-content-for-a-specific-section}

När e-postmeddelandet har skapats med AI Assistant från en e-postmall kanske du ändå vill ändra vissa delar av bilden, till exempel e-post eller text.

SCREENSHOT

Från det tidigare e-postmeddelandet som genererades är bilden av hälso- och sjukvårdsexperten inte helt korrekt, så du kanske vill instruera AI-assistenten att skapa en bild av en sjukvårdsexpert precis som en representation, om du inte har någon faktisk bild.

I så fall kanske du vill markera en del av e-postmeddelandet och sedan använda AI-assistenten för att skapa innehåll för det avsnittet. Markera bildinnehållet och klicka sedan på AI-assistenten.

SCREENSHOT

Ange relevanta uppgifter i uppmaningen, t.ex.&quot;generera en bild för en sjukvårdsexpert&quot; och lägg till eventuella anpassningar, om det behövs. Du kan också använda promptbiblioteket till höger om uppmaningen om du inte är säker på vilken uppmaning du ska ange.

När du klickar på&quot;Generera&quot; skapas flera varianter och du kan välja den som passar innehållet i e-postmeddelandet.

SCREENSHOT

På samma sätt som bilden kan andra delar av innehållet, till exempel text, ändras.

SCREENSHOT

## Skapa ett helt e-postmeddelande från en vald mall {#create-an-entire-email}

Det här alternativet är bara tillgängligt om e-postmeddelandet har skapats med en befintlig mall. Det här kan vara en standardmall som tillhandahålls av e-post-Designer, en sparad mall som redan har skapats av en marknadsförare eller en importerad mall som använder Importera HTML. Observera att det här alternativet inte är tillgängligt om du har valt&quot;Design från grunden&quot; för ditt e-postmeddelande.

När du väljer en viss mall, utan att markera någon komponent i mallen, klickar du på AI-assistentknappen i Designer New Email.

SCREENSHOT

Ange den relevanta uppmaningen och välj textinställningar, varumärkesresurser och eventuella bildinställningar som du vill ha för e-postmeddelandet.

SCREENSHOT

Om du vill generera bilder med Firefly väljer du Bildinställningar och aktiverar alternativet Skapa bilder med AI

SCREENSHOT

Välj lämpliga inställningar, t.ex. Innehållstyp, Färg och Ton, Ljus samt disposition för att skapa Gen-AI-bilder för e-postmeddelandet. Klicka på Generera för att generera varianter av e-postmeddelandet.

SCREENSHOT

Välj en av varianterna som ska förhandsgranskas genom att klicka på Förhandsgranska eller använd varianten för att spegla ändringen på arbetsytan.
