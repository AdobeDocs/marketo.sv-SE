---
title: understanding-my-tokens
description: Förstå mina token
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Förstå mina token

<br> 

Mina token är anpassade variabler som du kan skapa och använda i program- och kampanjmappar. De ser ut så här: `{{_my.Name of Token_}}`

## Exempel

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Om du vill komma åt och skapa Mina token väljer du program- eller kampanjmappen och går till [!UICONTROL My Tokens] -fliken. Dra och släpp en token på din [!UICONTROL Local Tokens] arbetsyta.

![Bild ett](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Namnen på Mina token kan inte ändras efter att de har sparats, så välj noga.

>[!NOTE]
>
>Mina token kommer inte att matchas när du skickar ett e-postmeddelande från Sales Insight på antingen Microsoft Dynamics eller Salesforce. endast standardtokens fylls i (Lead, Company, etc.). Standardvärden för tokens fungerar dock.

>[!NOTE]
>
>Länktoken fungerar inte i e-postmeddelanden med endast text.

## Kapslade token

När du skapar en ny token kan andra objekt i trädet referera till den. Du kan åsidosätta globala variabler på lägre nivåer i trädet. Det finns en namngivningsstruktur där token skapades för enkel hantering.

* **Lokal token:** Token skapades direkt i programmet eller mappen.
* **[Åsidosatt token:](/help/sky/override-an-inherited-my-token.md)** Token ärvdes, men ett undantag gjordes i programmet eller mappen.
* **Ärvd token:** Token skapades någonstans i ett program eller en mapp på en högre nivå.

Du hittar dessa tre typer under fliken **[!UICONTROL My Tokens]** i program- eller kampanjmappen.

![Bild två](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

När du flyttar program och mappar påverkas även tokens. Kontrollera alltid för att se till att referenser inte bryts under flyttningen.

>[!NOTE]
>
>Om e-postmeddelandet som skickas från ett engagemangsprogram är en underordnad e-postadress till ett standardprogram (d.v.s. inte lokal till ditt engagemangsprogram), löses alla Mina token som används i e-postmeddelandet från standardprogrammet där den underordnade e-postadressen finns.

## Tokenanvändning

Välj en variabel och klicka sedan på användningsikonen i det övre högra hörnet för att visa en lista med resurser som innehåller denna variabel.

![Bild tre](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Bild fyra](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Djupdykning**

Läs mer om alla Mina token:

* [CRM-kampanj](/help/sky/my-token-crm-campaign.md)
* [Datum](/help/sky/my-token-date.md)
* [Kalenderfil](/help/sky/my-token-calendar-file.md)
* [Bild](/help/sky/my-token-image.md)
* [Länk](/help/sky/my-token-link.md)
* [Nummer](/help/sky/my-token-number.md)
* [RTF](/help/sky/my-token-rich-text.md)
* [Poäng](/help/sky/my-token-score.md)
* [E-postskript](/help/sky/my-token-email-script.md)
* [Text](/help/sky/my-token-text.md)
