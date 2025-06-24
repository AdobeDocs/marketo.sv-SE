---
unique-page-id: 12983280
description: Versionsinformation -höst 17 - Marketo Docs - produktdokumentation
title: Versionsinformation - höst 17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Versionsinformation: höst 17 {#release-notes-fall}

Följande funktioner finns i höstutgåvan 17. Se om det finns funktioner i Marketo Edition.

Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion. Obs! Vissa av funktionerna i den här versionen har inte associerade artiklar. Om ett ämne har flera underrubriker placeras länkarna där.

## Systemtillförlitlighet {#system-reliability}

Vi har gjort ytterligare förbättringar av Marketo kärninfrastruktur, bland annat bättre sekvensering, färre avvikelser och förbättrad stabilitet för [!DNL Munchkin].

## SFDC Sync Performance {#sfdc-sync-performance}

Utnyttja den djupare och snabbare synkroniseringen i Marketo och [!DNL Salesforce]. Dataändringar som kräver satsvis uppdatering av konton eller leads kan delas upp i parallella köer för att undvika eftersläpningar. Händelser och uppgifter synkroniseras nu också upp till 50 % snabbare.

## Prestandaförbättringar för analyser {#analytics-performance-improvements}

De senaste infrastrukturförbättringarna ger ökad drifttid och stabilitet i Marketo rapporterings- och analysverktyg, vilket gör att du kan skapa ad hoc-rapporter snabbare.

## [Mottagarens tidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Med den här nya funktionen kan du nu lagra och leverera e-post enligt lokala tidszoner. E-post- och engagemangsprogram kan konfigureras så att de levereras i mottagarnas tidszoner, vilket eliminerar behovet av att skapa flera program - skicka en gång så håller Marketo automatiskt e-postmeddelandet tills rätt lokal tid. Lyft e-poststatistik, observera lokala rutiner och spara tid med ett enda program globalt.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Om du inte kan aktivera tidszonen för mottagare i dina e-post- och engagemangsprogram ännu, ska du inte få panik! Vi aktiverar den här funktionen gradvis för alla kunder.

## [Granska exempelmejl efter segment](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo har ett nytt alternativ för att välja ett segment när exempelmeddelanden skickas för granskning. Du behöver inte längre manuellt avgöra vilket segment ett lead tillhör, vilket gör det enklare att skicka e-postmeddelanden med dynamiskt innehåll till olika segment.

## [Anpassade frågor om LinkedIn-lead-generering](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Anpassa dina [!UICONTROL LinkedIn Lead Gen]-formulär för att samla in anpassade lead-attribut. Du kan nu ställa upp till tre anpassade frågor per formulär, välja mellan enradig textinmatning eller flervalsfrågor och mappa tillbaka till Marketo lead-fält.

## Slack Integration {#slack-integration}

Vi har släppt två funktioner som en del av vår nya integrering med Slack:

* Systemmeddelanden: Få Slack-meddelanden om viktiga händelser i din Marketo-instans, som aviseringar om aktuella kampanjstatus och eventuella problem som kräver omedelbar åtgärd.
* Intressanta ögonblick: När en Marketo Insight har utlösts av en känd person från ett försäljningskonto kan ledande ägare meddelas via Slack. Meddelanden innehåller information om lead samt detaljer om försäljningskontot.

## ABM-förbättringar {#abm-enhancements}

**[Visa konton utan kontakter](https://docs.marketo.com/x/fKCt)**

Marketo ABM synkroniserar nu och visar CRM-konton utan kontakter. Inkludera nya konton utan tidigare sälj- eller marknadsföringshistorik och följ upp framstegen genom att matcha efterföljande leads med kontona.

## ContentAI Analytics {#contentai-analytics}

**[Nytt listfilter för ABM-konto](https://docs.marketo.com/x/1BPG)**

Visa och jämför innehållsprestanda i kontolistor för ABM för att optimera befintligt innehåll. ContentAI visar dig:

* populärt innehåll visat
* toppkonverterat innehåll
* AI-baserat föreslaget innehåll för marknadsföringsaktiviteter

## Förbättringar i Personalization {#web-personalization-enhancements}

**[Tokens för webbkampanjer](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Tokens finns nu tillgängliga för användning inom webbkampanjer. Använd variabler för att leverera personaliserade meddelanden och innehåll för att öka engagemanget i era webbkampanjer.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Design Studio-bilder i Web Campaign Editor](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Spara tid genom att återanvända kreativa resurser och bilder i flera kanaler i Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integrering  {#integration}

**[API för e-postförhandsgranskning](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/email-scripting)**

Nu kan du förgranska e-post utanför Marketo via fjärranslutning, vilket förenklar processen för lokalisering av e-postinnehåll och minskar antalet fel.

**[Ersätt HTML API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/email-scripting)**

Utvecklare kan fjärruppdatera HTML-innehåll för e-postresurser, så att de kan arbeta i ett enda system för att underhålla resurser.
