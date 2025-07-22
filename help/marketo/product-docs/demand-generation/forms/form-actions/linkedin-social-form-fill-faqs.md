---
unique-page-id: 10098238
description: LinkedIn Social Form Fill FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om LinkedIn-fyllning av sociala formulär
hide: true
hidefromtoc: true
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!DNL LinkedIn] Vanliga frågor om ifyllnad av sociala formulär {#linkedin-social-form-fill-faqs}

Den reviderade API-principen för [!DNL LinkedIn] kräver att vi tar bort [!DNL LinkedIn] Social Form Fill från produkten.

## Viktiga saker att veta {#important-things-to-know}

* [!DNL LinkedIn] Knappar för ifyllning av sociala formulär kunde inte längre läggas till i Marketo den 28 april 2016

* Vi har tagit bort knappen [!DNL LinkedIn] för ifyllnad av sociala formulär från alla formulär där den var aktiverad

## Varför togs den här funktionen bort från min Marketo-prenumeration? {#why-was-this-functionality-removed-from-my-marketo-subscription}

LinkedIn gjorde några betydande ändringar i sitt utvecklarprogram. Som en del av dessa förändringar kan Marketo inte längre ge stöd för den här funktionaliteten för sina kunder.

## Vad hände om jag inte tog bort knapparna [!DNL LinkedIn] för ifyllnad av sociala formulär från formulär som hade sociala formulär aktiverat? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

Den 28 april 2016 tog vi bort knappen [!DNL LinkedIn] för ifyllnad av sociala formulär från formulär som fortfarande hade sociala formulär aktiverat.

## Jag har infogat den här funktionaliteten i formulär sedan vi blev Marketo-kund. Hur vet jag vilka formulär som använder [!DNL LinkedIn] ifyllning av sociala formulär? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Innan vi gjorde den här ändringen skickade vi ut meddelanden varje vecka till din inkorg med en lista över formulär som använde [!DNL LinkedIn] ifyllning av sociala formulär. Dessa aviseringar var avsedda att hjälpa dig att identifiera var du använde den här funktionen.

## Fungerar fortfarande knappar för delning via sociala medier i [!DNL LinkedIn]? {#do-linkedin-social-sharing-buttons-still-work}

Ja. Ändringen påverkar bara funktionen för ifyllning av sociala formulär i [!DNL LinkedIn].

## Fungerar [!DNL Facebook] och [!DNL Twitter] ifyllning av sociala formulär fortfarande? {#do-facebook-and-twitter-social-form-fill-still-work}

Ja. [!DNL Facebook] och [!DNL Twitter] ifyllning av sociala formulär har inte ändrats.

## Har det hänt något med de data som vi redan har hämtat via [!DNL LinkedIn] ifyllning av sociala formulär? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

Nej, dessa data har redan lagrats på personposten i Marketo och påverkades inte av den här ändringen.

## Var finns mer information om LinkedIns API-policy? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Följ den här länken om du vill veta mer om de ändringar som [!DNL LinkedIn] har gjort i deras API-princip: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## Hur kontaktar jag [!DNL LinkedIn] med frågor? {#how-can-i-contact-linkedin-with-questions}

Följ den här länken för att kontakta [!DNL LinkedIn] om deras marknadsföringslösningar: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Om Marketo tog bort denna funktionalitet från formulären den 28 april, förvandlades mina formulär och de berörda landningssidorna till utkastläge? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

Nej, formulären som vi har tagit bort den här funktionen från har publicerats.

## Om [!DNL LinkedIn] var mitt enda markerade nätverk, ändrar detta utseendet på mitt formulär? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

Nej, vi tar bara bort knappen [!DNL LinkedIn] från ditt formulär. När ifyllning av sociala formulär används i ett formulär skapas en behållare ovanför som innehåller knapparna för ifyllning av sociala formulär. Före den 28 april 2016, om [!DNL LinkedIn] var det enda alternativet, liknade behållarens utseende den här bilden:

![—](assets/one.png)

Efter den 28 april 2016 finns det nu en tom behållare längst upp i något formulär där [!DNL LinkedIn] ifyllning av sociala formulär har tagits bort:

![—](assets/two.png)

>[!NOTE]
>
>Bilderna ovan är till exempel bara. Detta kanske inte är exakt så som knappbehållaren för ifyllning av sociala formulär återges. Alla teckensnittsfärger, format osv. du har valt att påverka hur behållaren ser ut.

## Om [!DNL LinkedIn] var mitt enda markerade nätverk, hur tar jag bort den tomma behållaren ovanför mitt formulär? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

Du kan ta bort den tomma behållaren genom att redigera formuläret, markera [!DNL Facebook] eller [!DNL Twitter] som ett alternativ för ifyllning av sociala formulär och sedan avmarkera [!DNL Facebook] eller [!DNL Twitter] som ett alternativ för ifyllning av sociala formulär. Detta återställer de sociala alternativen i formulärfyllningsbehållaren och tar bort den från formuläret.
