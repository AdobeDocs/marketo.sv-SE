---
solution: Marketo Engage
product: marketo engage
title: Använda AI-assistenten
description: Utnyttja Adobe generativa AI-teknik för att lägga till användbar text och/eller bilder i e-postmeddelanden.
feature: Email Editor
exl-id: e07ed645-d8a3-483f-aa1f-f82bc9cb8634
source-git-commit: e9a412d0786a0dbeb6f743a90bcaf735032561a6
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Använda AI-assistenten {#use-the-ai-assistant}

AI-assistenten i Marketo Engage Email Designer hjälper dig att skapa aktuella, högpresterande och intuitiva e-postmeddelanden. Detta uppnås genom Adobe generativa AI-teknologi och ett bibliotek med Firefly för bildgenerering som hjälper till att skapa lämpligt innehåll för en viss individ/köpgrupp, marknadsföringssteg, kommunikationsstrategi, ton osv. Specifika varumärkesresurser kan också användas för att skapa innehåll.

>[!PREREQUISITES]
>
>AI-assistenten är inte aktiverad som standard. Du måste först godkänna villkoren för Core Gen-AI och de kompletterande villkoren för att använda Gen-AI-funktionen i e-postprogrammet för Designer. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

Det finns tre primära användningsområden för AI-assistenten:

* [Skapa en ämnesrad](#create-a-subject-line) för ditt e-postmeddelande
* [Skapa innehåll för ett visst avsnitt](#create-content-for-a-specific-section) i e-postmeddelandet
* [Skapa ett helt e-postmeddelande](#create-an-entire-email) från en markerad mall

## Skapa en ämnesrad {#create-a-subject-line}

När ett e-postmeddelande skapas med Designer New Email anger du en tillfällig ämnesrad.

![](assets/use-the-ai-assistant-1.png)

När e-postmeddelandet har skapats finns ämnesraden i kolumnen _Detaljer_ till höger. Klicka på AI-assistentknappen ( ![Filterikon](assets/icon-ai-assistant.png) ) bredvid om du vill ha hjälp med att skapa en ny ämnesrad med Gen AI-funktionen.

![](assets/use-the-ai-assistant-2.png)

Aktivera alternativet **Använd referensinnehåll** för AI-assistenten för att anpassa nytt innehåll baserat på det valda innehållet.

Ange uppmaningen att anpassa ämnesraden. Ange relevanta textinställningar och överför alla varumärkesresurser som du vill använda som referens för att skapa en lämplig ämnesrad.

![](assets/use-the-ai-assistant-3.png)

Textinställningarna omfattar:

<table><tbody>
  <tr>
    <td style="width:25%"><b>Buying Group</b></td>
    <td>Den specifika köpgrupp som ni riktar in er på (t.ex."Practitioner","Influencer","Decision Maker").</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Marknadsföringsresa</b></td>
    <td>Mottagare i ett visst stadium av marknadsföringsresan (t.ex. Discover, Evaluate, Commit).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Kommunikationsstrategi</b></td>
    <td>Syftet med kommunikationen (t.ex. brådskande frågor, socialt bevis, information).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Språk</b></td>
    <td>Det språk som du vill att ämnesraden ska skapas på.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Ton</b></td>
    <td>Ton som du vill att innehållet ska genereras i (t.ex. Inspiration, Exciting, Humorous).</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Emojis</b></td>
    <td>Gör att uttryckssymboler kan inkluderas i det genererade innehållet.</td>
  </tr>
</tbody>
</table>

När du klickar på **Generera** visas exempel som du kan välja bland:

![](assets/use-the-ai-assistant-4.png)

Du kan också överföra en varumärkesresurs för att använda innehåll i resursen som referens för att skapa ämnesraden.

![](assets/use-the-ai-assistant-5.png)

Om du vill välja en variant markerar du dess kryssruta och klickar på **Markera**. Du kan även ändra den genom att klicka på **Förfina**. Dessutom kan du ge feedback genom att klicka på reglagen uppåt eller nedåt så att Gen-AI-tekniken lär dig mer om dina önskemål.

När du har gjort ditt val fylls ämnesraden i i din e-postinformation.

![](assets/use-the-ai-assistant-6.png)

## Skapa innehåll för ett visst avsnitt i e-postmeddelandet {#create-content-for-a-specific-section}

När e-postmeddelandet har skapats kan du ändra vissa avsnitt, bilder eller text.

![](assets/use-the-ai-assistant-7.png)

I det här exemplet använder vi en vårdmall. Om den befintliga bilden av hälso- och sjukvårdsexperten inte uppfyller dina behov kan du instruera AI-assistenten att skapa en egen bild av en sjukvårdsexpert. Markera bara bildinnehållet och klicka sedan på AI-assistenten.

![](assets/use-the-ai-assistant-8.png)

Ange relevanta uppgifter i meddelandet, t.ex.&quot;generate an image for a medical expert&quot;, och lägg till önskad anpassning. Du kan också använda promptbiblioteket (till höger om uppmaningen) om du inte är säker på vad du ska ange.

När du har klickat på **Generera** skapas flera varianter att välja mellan.

![](assets/use-the-ai-assistant-9.png)

Textdelar av e-postmeddelandet kan också ändras på samma sätt som bilden.

![](assets/use-the-ai-assistant-10.png)

## Skapa ett helt e-postmeddelande från en vald mall {#create-an-entire-email}

Det här alternativet är bara tillgängligt om e-postmeddelandet har skapats med en befintlig mall. Det kan vara en standardmall som tillhandahålls av e-post-Designer, en sparad mall som du redan har skapat eller en importerad mall som använder alternativet Importera HTML. Det här alternativet är inte tillgängligt om du väljer [Designa från grunden](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#design-from-scratch) för ditt e-postmeddelande.

Välj en mall utan att markera någon komponent i mallen och klicka på AI-assistentknappen i e-postens Designer.

![](assets/use-the-ai-assistant-11.png)

Ange den relevanta uppmaningen och välj textinställningar, varumärkesresurser och eventuella bildinställningar som du vill använda för e-postmeddelandet.

![](assets/use-the-ai-assistant-12.png)

Om du vill generera bilder med Firefly väljer du Bildinställningar och väljer alternativet **Generera bilder med AI**.

![](assets/use-the-ai-assistant-13.png)

Välj önskad _innehållstyp_, _färg och ton_, _ljus_ och _komposition_ för att skapa Gen-AI-bilder för e-postmeddelandet. Klicka på **Generera** när du är klar.

![](assets/use-the-ai-assistant-14.png)

Se hur en variant kommer att se ut i ditt e-postmeddelande genom att klicka på **Förhandsgranska**. Välj en variation genom att klicka på **Använd**.
