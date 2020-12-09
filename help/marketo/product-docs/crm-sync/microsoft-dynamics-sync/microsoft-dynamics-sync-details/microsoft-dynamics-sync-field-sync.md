---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - fältsynkronisering
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Fältsynkronisering {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Marketo to Dynamics sync är superkraftfull. Här är detaljerna.

## Hur synkroniseras fältinformation mellan de två systemen? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är dubbelriktad för lead- och kontaktentiteter. Om du ändrar ett lead eller en kontakt i Dynamics eller en person i Marketo återspeglas dina uppdateringar i båda systemen.

Synkroniseringen är envägs för konton, användare, affärstillfällen, team och anpassade entiteter: Dynamics till Marketo. Om du gör ändringar i de här enheterna i Dynamics återspeglas dina uppdateringar i Marketo.

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Trots att detta är sällsynt kommer Marketo att vinna för människor (leads) och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM). För enkelriktade synkroniseringsenheter vinner Dynamics alltid.

## Kan jag skapa ett fält i Dynamics med Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Nej, det stöds inte för närvarande.

## Jag skapade ett fält i Dynamics. Kan jag synkronisera den till Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, du kan [synkronisera fältet](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) så länge din synkroniseringsanvändare har åtkomst till det i Dynamics.

Vilka fält synkroniseras med Marketo?

Du kan [välja fält som ska synkroniseras](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) under installationen.

## Vad händer om jag behöver lägga till ett anpassat fält efter att Marketo och Dynamics har synkroniserats? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Du kan lägga till fält när som helst och förvänta dig att data uppdateras från Dynamics till Marketo. Mer information finns i [Använda snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) .

>[!MORELIKETHIS]
>
>* [Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



