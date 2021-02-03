---
unique-page-id: 7515133
description: SFDC-synkronisering - Sammanfoga en lead/kontakt/person - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Sammanfoga en lead/kontakt/person
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# SFDC-synkronisering: Sammanfoga en lead/kontakt/person {#sfdc-sync-merging-a-lead-contact-person}

Ibland är det bäst att bara lista reglerna. Här är vi:

* När du sammanfogar två leads i **Salesforce** anger den normala synkroniseringen Marketo och leads sammanfogas automatiskt som personer i Marketo.
* När du sammanfogar två personer i **Marketo** anropas i själva verket samma process som när de sammanfogas som leads i Salesforce. Det fungerar fortfarande automatiskt.
* Att sammanfoga ett **lead (person) till en kontakt** fungerar på samma sätt. Du får en enda kontakt på båda sidor.
* Standardpoängen sammanfogas vid sammanslagningen.

>[!NOTE]
>
>Om du sammanfogar 3 leads (personer) med poängen 10 var, får du resultatet 1 lead (person) med poängen 30.

* Fältvärden i konflikt hämtas från den&quot;vinnande posten&quot;. (Post = den resulterande lead eller kontakten)
* Om den&quot;förlorade posten&quot; (den som försvinner) hade ett värde och den vinnande posten inte har något, behåller vi den förlorade posten. Med andra ord:&quot;Vissa värden är bättre än inga värden.&quot;
* Alla aktivitetsloggsobjekt sammanfogas.

>[!NOTE]
>
>Djupdykning om du vill ha mer information om [att sammanfoga personer i Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
