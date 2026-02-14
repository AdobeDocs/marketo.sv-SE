---
description: Konfigurera Design Studio-avsnittet för din nya Marketo Engage-instans.
title: New Instance Best Practices - Design Studio Checklist
feature: Getting Started
exl-id: 070ee235-dad0-4627-bac0-14bf0174bb03
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# New Instance Best Practices: Design Studio Checklist {#new-instance-best-practices-design-studio-checklist}

I Design Studio-delen finns de återanvändbara&quot;globala resurserna&quot;. Skapa globala resurser som din organisation tänker använda i program, använd en konsekvent namnkonvention och ordna dem i undermapparna för enkla sökningar.

Kom ihåg att [hämta checklistorna](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) och spåra dina framsteg.

## Landningssidor {#landing-pages}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Globala landningssidor</td>
    <td><li>Skapa <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages#product-docs" target="_blank">globala landningssidor (frihand/guidad)</a>.</li>
    <li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups" target="_blank">Skapa en testsida</a> för att A/B-testa den vinnande landningssidmallen (om tillämpligt).</li></td>
  </tr>
  <tr>
    <td>Mallar</td>
    <td><li>Skapa en design för globala landningssidor.</li></td>
  </tr>
  <tr>
    <td>Sekretess och efterlevnad</td>
    <td><li>Skapa en sidfot med <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page" target="_blank">Utdrag</a> eller <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-text-and-tokens-to-a-landing-page#add-a-token-to-your-landing-page" target="_blank">Token</a> på dina landningssidor för sekretessefterlevnad.</li></td>
  </tr>
</tbody>
</table>

## Forms {#forms}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Global Forms</td>
    <td><li>Konfigurera <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/forms/creating-a-form/create-a-form#product-docs" target="_blank">globala formulär</a> för användningsfall som prenumerationsinställningar, hämtningar av Gated-innehåll, demonstrationsförfrågningar, webbinarieregistreringar osv.</li></td>
  </tr>
  <tr>
    <td>Sekretess och efterlevnad</td>
    <td><li>Behåll dina formulär <a href="https://business.adobe.com/se/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">enligt den allmänna dataskyddsförordningen (GDPR)</a>.</li></td>
  </tr>
  <tr>
    <td>Datainsamling</td>
    <td><li>Överväg att tillämpa plocklistor på <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/forms/creating-a-form/add-a-field-to-a-form#product-docs" target="_blank">formulärfälten</a> i stället för öppna textfält för att förhindra röriga data.</li></td>
  </tr>
</tbody>
</table>

## E-post {#emails}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Globala e-postmeddelanden</td>
    <td><li>Skapa globala e-postmeddelanden.</li></td>
  </tr>
  <tr>
    <td>Mallar</td>
    <td><li>Designa en modulbaserad <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/email-marketing/general/email-editor-2/create-an-email-template" target="_blank">e-postmall</a> med en designer/utvecklare, eller använd din egen HTML.</li>
    <li>Skapa en testad e-postmall för att A/B-testa den vinnande mallen (om tillämpligt).</li></td>
  </tr>
  <tr>
    <td>Sekretess och efterlevnad</td>
    <td><li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email" target="_blank">Lägg till fragment</a> i e-postmallarna för att styra återanvändbara block som copyright year, global location och kompatibilitetsspecifikt språk.</li>
    <li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email" target="_blank">Lägg till token</a> om du vill anpassa innehåll baserat på målgruppen.</li></td>
  </tr>
</tbody>
</table>

## Fragment {#snippets}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Fragment</td>
    <td><li>Skapa <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet#product-docs" target="_blank">Kodavsnitt</a> om du vill ha återanvändbara innehållsblock som kan användas i flera fall, t.ex. kontaktinformation, länkar till sociala medier, varumärkesinformation och sekretess- och efterlevnadsinformation i dina e-postmeddelanden och landningssidor.</li></td>
  </tr>
</tbody>
</table>

## Bilder och filer {#images-and-files}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Namnkonventioner</td>
    <td><li>Använd konsekventa namnkonventioner för bilder och filer.</li>
    <br>Exempel:
    <br><ul><li>Namngivningskonvention för filer: Namn på tillgångar (t.ex. White-Paper-Evaluating-Cloud-Computing-get-your-Board-on-Board)</li>
    <p><li>Konvention om namngivning av bilder: namn på bildtyp-tillgångar (t.ex. miniatyrbilder-vit-papper-utvärdering-cloud-computing-get-your-board-on-board)</li></td>
  </tr>
</tbody>
</table>

## Organisation {#organization}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Mappstruktur </td>
    <td><li>Skapa undermappar för varje typ av resurs och <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders" target="_blank">ordna globala resurser</a> (t.ex. konversationsflöden, e-postmallar, e-post, formulär, bilder och filer, landningssidor, landningssidmallar, textutdrag osv.) på rätt sätt.</li></td>
  </tr>
</tbody>
</table>
