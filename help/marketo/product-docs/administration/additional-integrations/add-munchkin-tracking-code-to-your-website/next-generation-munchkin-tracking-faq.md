---
unique-page-id: 10096583
description: "Nästa generation [!DNL Munchkin] Spåra vanliga frågor - Marketo Docs - produktdokumentation"
title: "Nästa generation [!DNL Munchkin] Vanliga frågor om spårning"
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 1a6f029b8c9665ecd7fcc066004d88ee6c915505
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# Nästa generation [!DNL Munchkin] Vanliga frågor om spårning {#next-generation-munchkin-tracking-faq}

Vi är glada över att kunna meddela att vi snart kommer att påbörja en fasad lansering av nästa generations webbspårningsteknik.

Här är det viktigaste att veta:

* Vi tar bort filtret&quot;Är anonym&quot; med vår Q1-version (redan klar)
* Vi ökar antalet webbhändelser (Besök webbsida, Klickad länk på webbsida) som kan importeras
* Dina [!DNL Munchkin] så ingen uppdatering krävs

## När kommer min Marketo-prenumeration att vara aktiverad [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Vi har inget exakt datum än, men kom tillbaka hit för att få uppdateringar.

## Måste jag göra några ändringar i [!DNL Munchkin] spårar du på min webbplats? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Nej. The [!DNL Munchkin] spårningskoden förblir densamma. Inga ändringar behöver göras på webbplatsen.

>[!NOTE]
>
>Den här ändringen påverkar inte webbpersonalisering (anpassning i realtid). Det fortsätter att identifiera anonyma och kända webbbesökare och personalisera innehåll i realtid för dessa besökare.

## Varför tog Marketo bort filtret&quot;Är anonym&quot; från smarta listor? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Vi ändrade hur anonyma människor interagerar med smarta kampanjer. Förut gick de igenom en smart kampanj, precis som kända människor. Filtret &quot;Är anonym&quot; användes för att ange att bara kända eller bara anonyma personer flödar genom kampanjen.

Med [!DNL Munchkin] V2 kommer vi att fortsätta att spåra all anonym verksamhet. Du kan dock inte längre använda filter på anonyma personer. Vid konverteringen (när personen blir känd i Marketo) läggs alla aktiviteter som inträffade när personen var anonym till i personaktivitetsloggen och i nuläget flödar de genom de kampanjer personen är berättigad till.

Om du redan använder det här filtret i en smart lista (till exempel i en smart kampanj eller en rapport) tas det inte automatiskt bort från den smarta listan. Mer information finns nedan.

>[!NOTE]
>
>**Utlösare**: Besök webbsidan, webbsidan är prissättningssida\
>**Flöde**: Ändra bakgrundsmusik +10 och intressant stund
>**Webb**: Visad prissida
>
>Med [!DNL Munchkin] V2, om en anonym person besöker prissidan, så deltar hon inte i kampanjen direkt. När den anonyma personen blir känd ska vi genomföra kampanjen mot henne. Hon kommer att:
>
>* Få 10 poäng
>
>* Ha webbsidesaktiviteten inställd på rätt datum (när hon faktiskt besökte den)
>
>* Jag vill att en intressant stund ska registreras för henne (med det datum då hon faktiskt besökte sidan, inte när hon blev känd)
>
>* Logga aktiviteten Ny person, som den är idag


## Vad händer med mina smarta listor som redan har filtret&quot;Är anonym&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Om du har gamla smarta kampanjer med en smart lista som innehåller filtret&quot;Är anonym&quot; efter vinterutgåvan 16 kommer en av två saker att hända:

1. Om den smarta listan har filtret &quot;Är anonym = falsk&quot; händer ingenting. Vi kommer bara att ignorera det.
1. Om den smarta listan har filtret &quot;Är anonym = Sant&quot; kommer kampanjen att misslyckas och du får ett meddelande.

## Jag har använt Marketo ett tag. Hur vet jag vilken av mina kampanjer som använder filtret&quot;Är anonym&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Innan vi gjorde den här ändringen skickade vi ut flera meddelanden varje vecka till din inkorg med en lista över smarta listor, smarta kampanjer och rapporter som använder filtret&quot;Är anonym&quot;. Dessa kan hjälpa dig att identifiera var du använder det här filtret.

Granska dem och identifiera var ni har inställningen &quot;Är anonym&quot; till True, eftersom det är de kampanjer som påverkas. Oftast använder kunderna den här inställningen för någon form av poängsättning. Se exemplet ovan för att förstå hur dessa kampanjer kommer att fungera nu.

## Jag vill ha mer detaljerad dokumentation. Var kan jag hitta den? {#id-like-more-detailed-documentation-where-can-i-find-it}

Kolla in länkarna:

[Översikt över anonyma leaduppgraderingar](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Anonyma leaduppgraderingar - ändringar i Marketo användargränssnitt](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Anonyma leaduppgraderingar - kundåtgärd krävs](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Anonyma leaduppgraderingar - analysrapporter](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Anonyma leaduppgraderingar - versionsschema](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Anonyma leaduppgraderingar - under molnet](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Anonym leadmarknadsföring till känd lead - [!DNL Munchkin] V2-beteende](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Jag har fler frågor! Hur får jag svar på dem? {#i-have-more-questions-how-do-i-get-them-answered}

Var vänlig och kontakta [community](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. De kommer gärna att besvara dina frågor.
