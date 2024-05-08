---
unique-page-id: 10098238
description: LinkedIn Social Form Fill FAQ - Marketo Docs - produktdokumentation
title: LinkedIn Social Form Fill - frågor och svar
hide: true
hidefromtoc: true
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
feature: Forms
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# LinkedIn Social Form Fill - frågor och svar {#linkedin-social-form-fill-faqs}

LinkedIn reviderade API-policy kräver att vi tar bort LinkedIn Social Form Fill från vår produkt.

## Viktiga saker att veta {#important-things-to-know}

* LinkedIn-knappar för ifyllning av sociala formulär kunde inte längre läggas till i Marketo den 28 april 2016

* Vi har tagit bort LinkedIn-knappen för ifyllnad av sociala formulär från alla formulär där den var aktiverad

## Varför togs den här funktionen bort från min Marketo-prenumeration? {#why-was-this-functionality-removed-from-my-marketo-subscription}

LinkedIn har gjort betydande ändringar i sitt utvecklarprogram. Som en del av dessa förändringar kan Marketo inte längre ge stöd för den här funktionaliteten för sina kunder.

## Vad hände om jag inte tog bort LinkedIn Social Form Fill-knapparna från formulären som hade Social Form aktiverat? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

Den 28 april 2016 tog vi bort LinkedIn Social Form Fill från formulär som fortfarande hade Social Form aktiverat.

## Jag har infogat den här funktionaliteten i formulär sedan vi blev Marketo-kund. Hur vet jag vilka formulär som använder LinkedIn Social Form Fill? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Innan vi gjorde den här ändringen skickade vi ut veckovisa meddelanden till Inkorgen med en lista över formulär som använde LinkedIn Social Form Fill. Dessa aviseringar var avsedda att hjälpa dig att identifiera var du använde den här funktionen.

## Fungerar LinkedIn Social Sharing-knappar fortfarande? {#do-linkedin-social-sharing-buttons-still-work}

Ja. Ändringen påverkar bara LinkedIn funktion för ifyllnad av sociala formulär.

## Fungerar Facebook och Twitter Social Form Fill fortfarande? {#do-facebook-and-twitter-social-form-fill-still-work}

Ja. Facebook och Twitter Social Form Fill har inte ändrats.

## Har det hänt något med de data vi redan har samlat in via LinkedIn Social Form Fill? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

Nej, dessa data har redan lagrats på personposten i Marketo och påverkades inte av den här ändringen.

## Var finns mer information om LinkedIn API-policy? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Följ den här länken om du vill veta mer om de ändringar som LinkedIn har gjort i deras API-policy: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## Hur kontaktar jag LinkedIn med frågor? {#how-can-i-contact-linkedin-with-questions}

Följ den här länken för att kontakta LinkedIn om deras marknadsföringslösningar: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Om Marketo tog bort denna funktionalitet från formulären den 28 april, förvandlades mina formulär och de berörda landningssidorna till utkastläge? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

Nej, formulären som vi har tagit bort den här funktionen från har publicerats.

## Om LinkedIn var mitt enda valda nätverk, kommer detta att ändra utseendet på mitt formulär? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

Nej, vi tar bara bort LinkedIn-knappen från ditt formulär. När ifyllning av sociala formulär används i ett formulär skapas en behållare ovanför som innehåller knapparna för ifyllning av sociala formulär. Före den 28 april 2016, om LinkedIn var det enda alternativet, liknade behållarens utseende den här bilden:

![—](assets/one.png)

Efter den 28 april 2016 finns det nu en tom behållare längst upp i alla formulär där LinkedIn Social Form Fill har tagits bort:

![—](assets/two.png)

>[!NOTE]
>
>Bilderna ovan är till exempel bara. Detta kanske inte är exakt så som knappbehållaren för ifyllning av sociala formulär återges. Alla teckensnittsfärger, format osv. du har valt att påverka hur behållaren ser ut.

## Hur tar jag bort den tomma behållaren ovanför mitt formulär om LinkedIn var mitt enda valda nätverk? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

Du kan ta bort den tomma behållaren genom att redigera formuläret, välja Facebook eller Twitter som ett alternativ för ifyllning av sociala formulär och sedan avmarkera Facebook eller Twitter som ett alternativ för ifyllning av sociala formulär. Detta återställer de sociala alternativen i formulärfyllningsbehållaren och tar bort den från formuläret.
