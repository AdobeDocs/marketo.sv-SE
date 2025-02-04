---
title: Content Accelerator doc
description: Lär dig hur..
hide: true
hidefromtoc: true
source-git-commit: 1676c9049c61a637faede4751ea49bbcfa018be5
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Content Accelerator doc {#connect-experience-manager-doc}

Content Accelerator (med Gen-AI-funktioner)

Content Accelerator eller AI Assistant är en funktionalitet i New Email Designer som hjälper marknadsförare att skapa aktuella, högpresterande och intuitiva e-postmeddelanden på ett produktivt sätt. Detta uppnås genom Adobe generative AI-teknik och ett bibliotek med snabbmeddelanden tillsammans med Firefly för bildgenerering som hjälper marknadsförarna att skapa lämpligt innehåll för en viss individ/köpgrupp, marknadsföringsresa, kommunikationsstrategi, ton och så vidare. Specifika varumärkesresurser kan också användas för att skapa innehåll med hjälp av indata från dessa varumärkesresurser.

Den här funktionen är endast aktiverad för kunder som har signerat Core Gen-AI-villkoren och som har erbjudits ytterligare villkor för att använda Gen-AI-funktionen i New Email Designer. Kontakta din kontorepresentant för att få tillgång till den här funktionen. Detta är inte tillgängligt som standard med nya e-post-Designer.

Content Accelerator kan användas för tre primära användningsområden:

* Skapa en ämnesrad för ditt e-postmeddelande
* Skapa ett helt e-postmeddelande från en markerad mall
* Skapa innehåll för ett visst avsnitt i e-postmeddelandet

## Skapa en ämnesrad {#creating-a-subject-line}

När du skapar ett e-postmeddelande med Designer New Email kan du ange en tillfällig ämnesrad.

SCREENSHOT

När e-postmeddelandet har skapats ska ämnesraden visas på fliken Information till höger. Bredvid ämnesraden finns en AI-assistentknapp som hjälper marknadsförarna att generera ämnesraden med hjälp av Gen AI-funktionen.

När du klickar på knappen öppnas följande skärm för att visa alternativ för att anpassa genereringen av ämnesraden.

SCREENSHOT

Om du redan har använt en ämnesrad och vill använda den som referens för genereringen, växlar du till knappen &quot;Använd referensinnehåll&quot;.

Ange uppmaningen att anpassa ämnesraden. Ange relevanta textinställningar och överför alla varumärkesresurser som du vill använda som referens för att skapa en lämplig ämnesrad.

SCREENSHOT

Textinställningarna omfattar:

<table><tbody>
  <tr>
    <td><b>Buying Group</b></td>
    <td>Den specifika inköpsgrupp ni riktar er mot, t.ex. påverkare, beslutsfattare osv.</td>
  </tr>
  <tr>
    <td><b>Marknadsföringsresa</b></td>
    <td>Mottagare i en viss fas av marknadsföringsresan, t.ex. Discover, Evaluate, Commit.</td>
  </tr>
  <tr>
    <td><b>Kommunikationsstrategi</b></td>
    <td>Målet med kommunikationen, till exempel Urgent, Social Proof, Informative</td>
  </tr>
  <tr>
    <td><b>Språk</b></td>
    <td>Det språk som du vill att ämnesraden ska skapas på.</td>
  </tr>
  <tr>
    <td><b>Ton</b></td>
    <td>Ton där du vill att innehållet ska skapas, t.ex. inspiration, spännande, humoristiskt osv.</td>
  </tr>
  <tr>
    <td><b>Emojis</b></td>
    <td>Markera det här alternativet om du vill att känslolägesikoner ska inkluderas i genereringen.</td>
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


## Skapa innehåll för specifika avsnitt i e-postmeddelandet {#create-content-for-a-specific-section}

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
