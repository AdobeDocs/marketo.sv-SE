---
description: Översikt över Engagement Map - Marketo Docs - produktdokumentation
title: Översikt över Engagement Map
exl-id: 01cb283d-06c2-4a99-86a9-39dea9550c08
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Översikt över Engagement Map {#engagement-map-overview}

Med Engagement Map kan ni visualisera era smarta kampanjer intuitivt. Den är helt bakåtkompatibel med alla befintliga Marketo Engage Smart Campaigns, utan att några nuvarande funktioner går förlorade.

>[!NOTE]
>
>Engagement Map är för närvarande tillgängligt i smarta kampanjer. Det är inte tillgängligt i Program.

![](assets/engagement-map-overview-1.png)

## Åtkomst till engagemangskarta {#accessing-engagement-map}

Navigera till en befintlig kampanj och klicka på knappen **Åtagandekarta** .

![](assets/engagement-map-overview-2.png)

När du är på Engagement Map visas två flikar: [Engagement Map](/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-tab.md){target="_blank"} och [Settings](/help/marketo/product-docs/core-marketo-concepts/engagement-map/settings-tab.md){target="_blank"}.

![](assets/engagement-map-overview-3.png)

## Kortbeskrivningar {#card-descriptions}

**Utlösare**: I kampanjer som innehåller utlösare har kartan ett kort för utlösaröversikt. Om du klickar på den visas ett kort för varje utlösare samt en utfällbar panel med ytterligare information.

**Filter**: I kampanjer som innehåller filter kommer kartan att innehålla ett filteröversiktskort. Om du klickar på den visas en utfällbar panel med ytterligare information om varje filter.

**Flödessteg**: Varje kampanj kommer att innehålla ett kort för varje flödessteg. Om du klickar på dem visas en utfällbar panel med ytterligare information.

**Alternativ**: Om ett flödessteg innehåller ett eller flera alternativ visas ett kort för varje val när du klickar på flödeskortet, samt en utfällbar panel med ytterligare information.

## Kapslade kampanjer {#nested-campaigns}

* Om en kampanj innehåller ett Request- eller Execute Campaign-flödessteg visas information om den kampanj som anropas samt en utfällbar panel med ytterligare information om du klickar på flödeskortet.

* Om en kampanj innehåller ett Request- eller Execute Campaign-flödessteg med alternativ, visas ett kort för varje val när du klickar på flödeskortet, samt en utfällbar panel med mer information om alternativen. Om du klickar på varje alternativkort visas information om den kampanj som anropas samt en utfällbar panel med mer information.

* Om någon av de kapslade kampanjerna dessutom har ett flödessteg för att begära eller köra kampanj, visas information om kampanjen om du klickar på flödeskortet. Detsamma gäller när flödessteget innehåller alternativ.

## Övre navigering {#top-navigation}

Den övre navigeringen innehåller följande funktioner:

* Kampanjnamn och åtkomst till&quot;Redigera kampanj&quot; modal, du kan redigera kampanjnamnet och beskrivningen här.

* Kampanjstatus och kampanjtyp visas under kampanjnamnet

* Knappen Aktivera/inaktivera för utlösarkampanjer

* Redigera smart lista - du kommer att navigeras till gränssnittet Smart lista på en ny flik där du kan lägga till eller redigera filter och/eller utlösare

* Redigera flöde - du kommer att navigeras till Flödesgränssnittet på en ny flik där du kan lägga till eller redigera dina flödessteg

* Export - Detta hämtar en bild av kampanjvisualiseringen. Den nedladdade versionen återspeglar alla grenar som du har expanderat

* Visa kampanjmedlemmar - En ny flik med information om kampanjmedlemmar öppnas.

>[!NOTE]
>
>Ändringar som görs på en öppen smart lista och Flödesflik visas på fliken Engagement Map när du uppdaterar. Den uppdateras inte automatiskt. Uppdateringar och redigeringar som sparas automatiskt visas när fliken för aktivitetskartan uppdateras.

## Vanliga frågor och svar {#faq}

**Måste jag återskapa alla mina kampanjer i Engagement Map?**

Nej. Engagement Map har fullständig bakåtkompatibilitet. Med en enkel musklickning kan ni se alla era befintliga kampanjer i gränssnittet för den visuella engagemangskartan.

**Betyder det att Engagement Map finns i Marketo Engage att jag förlorar åtkomsten till mappstrukturen och måste lära mig hur jag skapar en smart kampanj igen?**

Nej. Det fina med Engagement Map är att det ger er det bästa av två världar; det kompletterar det sätt på vilket ni bygger kampanjer just nu. Alla användare kommer fortfarande att få tillgång till Marketo Engage kraftfulla funktioner, som nu kompletteras med tydlig grafik.

**Är Engagement Map ett betalt tillägg?**

Nej. Alla befintliga och nya Marketo Engage-användare under alla prenumerationer har tillgång till den här kostnadsfria funktionen.

**Är det jag som är Marketo Engage-administratör som ansvarar för att aktivera/inaktivera Engagement Map?**

Nej. Engagement Map kommer att vara tillgängligt för alla användare i deras instanser. Du kan inte aktivera/inaktivera den för vissa användare, arbetsytor osv.

**Hur skiljer sig detta från andra visuella verktyg?**

Det finns tre viktiga saker som skiljer Engagement Map åt:

* Flexibilitet: Hantera och validera enkelt sammankopplade eller djupt inkapslade kampanjer med visualisering.

* Funktion: Alla bilder är utanför ramarna, vilket gör dem enklare att använda. Med den kapslade strukturen kan du dyka in och få hela bilden.

* Styrka: Du behåller alla finesser i Marketo Engage, nu i ett visuellt format.

>[!MORELIKETHIS]
>
>* [Fliken Åtagandekarta](/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-tab.md){target="_blank"}
>* [Fliken Inställningar](/help/marketo/product-docs/core-marketo-concepts/engagement-map/settings-tab.md){target="_blank"}
