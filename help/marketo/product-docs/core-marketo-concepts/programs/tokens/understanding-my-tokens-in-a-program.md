---
unique-page-id: 1147114
description: Förstå mina token i ett program - Marketo Docs - produktdokumentation
title: Förstå mina token i ett program
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Förstå mina token i ett program {#understanding-my-tokens-in-a-program}

En variabel är en variabel som du kan använda i e-postmeddelanden, landningssidor och smarta kampanjer för att göra livet enklare.

Förutom Mina token kan du även använda alla inbyggda tokens i dina program. Ta en titt på [Översikt över token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

## Mina token  {#my-tokens}

Mina token är anpassade variabler som alla kan skapa. Lokalt är de [skapade](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} antingen i kampanjmappar eller i program.

Mina token visas så här: `{{my.Name Of Token}}`

Exempel:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table>
 <thead>
  <tr>
   <th>Tokentyp</th>
   <th>Beskrivning</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Kalenderfil <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Använd den här token för att <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">lägga till en kalenderhändelsefil (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> i dina e-postmeddelanden och landningssidor.</td>
  </tr>
  <tr>
   <td><p>Datum <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td>
   <td>Denna token innehåller ett datumvärde. Datumet visas som årsdag (t.ex. 2016-05-23).</td>
  </tr>
  <tr>
   <td>E-postmeddelande <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Använd denna token för att köra ett Velocity-skript i dina e-postmeddelanden. Läs mer <a href="https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/email-scripting" title="Följ länk" rel="nofollow">här</a>. </td>
  </tr>
  <tr>
   <td>Nummer <span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td>
   <td>Ett heltal. Den kan till och med vara negativ.</td>
  </tr>
  <tr>
   <td>RTF <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Det här är HTML. Använd det i e-postmeddelanden och på landningssidor.</td>
  </tr>
  <tr>
   <td>Poäng <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Använd den här token i <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">Ändra poängflödessteget</a>. </td>
  </tr>
  <tr>
   <td colspan="1">SFDC Campaign <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td>
   <td colspan="1">Använd den här variabeln för att tillåta att leads som blir en del av ett Marketo-program även läggs till i det som SFDC Campaign läggs till.</td>
  </tr>
  <tr>
   <td>Text <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Bara lite text. Använd det när HTML är överdrivet. Storleksgränsen för texttoken är 524 288 tecken (UTF-8), eller 2 MB.</td>
  </tr>
 </tbody>
</table>

>[!CAUTION]
>
>Mina token kommer inte att matchas när du skickar ett e-postmeddelande från Sales Insight på antingen [!DNL Microsoft Dynamics] eller [!DNL Salesforce]. Endast standardtokens fylls i (Lead, Company osv.). Standardvärden för tokens _fungerar dock_.

## Kapslade token {#nesting-tokens}

När du skapar en ny token kan andra objekt i trädet referera till den. Det finns en namngivningsstruktur där token skapades för enkel hantering.

* **Lokal token:** Token skapades direkt i programmet eller mappen.
* **Ärvd token:** Token skapades upp trädet någonstans i ett program eller en mapp på en högre nivå.
* **Åsidosatt token:** Token ärvdes och någon gjorde sedan ett undantag i det här programmet eller den här mappen.

Du kan göra globala variabler och sedan åsidosätta dem på lägre nivåer i trädet.

När du flyttar program och mappar påverkas även tokens. Kontrollera alltid för att se till att referenser inte bryts under flyttningen.

>[!IMPORTANT]
>
>Kapslade token stöds inte i [gruppkampanjer](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md#batch-campaign){target="_blank"}.

>[!NOTE]
>
>Om e-postmeddelandet som du skickar från ett engagemangsprogram är en underordnad e-postadress till ett standardprogram (inte lokal till ditt engagemangsprogram) matchas alla Mina token som används i e-postmeddelandet från standardprogrammet där den underordnade e-postadressen finns.

>[!MORELIKETHIS]
>
>* [Översikt över token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Hantera mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
