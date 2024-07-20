---
unique-page-id: 2953188
description: Inkommande filter - Marketo Docs - produktdokumentation
title: Inkommande filter
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Inkommande filter {#inferred-filters}

[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} cookies och placerar dem i systemet när någon besöker din webbplats. Vi söker upp deras IP-adresser i en särskild databas och hittar all slags information.

>[!NOTE]
>
>Vi uppdaterar regelbundet databasen som används för IP-adresssökningar för att säkerställa att de härledda fältsvärdena förblir aktuella. Databasuppdateringar kan medföra nya härledda fältvärden som du kan behöva lägga till i filterdefinitioner för smarta listor.
>
>Databasuppdateringar kan utföras under en [Marketo Engage-produktversion](/help/marketo/release-notes/release-schedule.md){target="_blank"}. När en uppdatering görs innehåller versionsinformationen för [Marketo Engage ](/help/marketo/release-notes/current.md){target="_blank"} en förklaring till eventuella ändringar i härledda fältvärden.

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

När du använder något av de här filtren i en smart lista kommer resultatet att ge personer den här slutna informationen.

>[!TIP]
>
>Använd dessa filter i en webbaktivitetsrapport. Använd säljarnas territorier och prenumerera på en anpassad daglig rapport med webbplatsbesökare de senaste 24 timmarna. De kommer att älska det!
>
>* Besökt webbsida - de senaste 24 timmarna
>* Den härledda staten är [välj deras territorium]

Dessa anonyma besökare konverteras automatiskt till personer när de klickar på en e-postlänk eller fyller i ett formulär. De behåller dock all information som de kommit fram till.

>[!NOTE]
>
>Läs mer om [anonym aktivitet och leads](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}.
