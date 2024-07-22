---
unique-page-id: 11378814
description: Smarta kontolistor - Marketo Docs - produktdokumentation
title: Smarta kontouppsättningar
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Smarta kontouppsättningar {#account-smart-lists}

Så här identifierar du snabbt och korrekt dina värdefulla konton.

>[!NOTE]
>
>Den här funktionen är bara tillgänglig för dem som har både tillägget för målkontohantering och en licensierad TAM.

## Skapa en smart kontolista {#create-an-account-smart-list}

1. Gå till **Marknadsföringsaktiviteter** i Marketo.

   ![](assets/account-smart-lists-1.png)

1. Hitta och välj önskat program.

   ![](assets/account-smart-lists-2.png)

1. Klicka på listrutan **Ny** och välj **Ny lokal resurs**.

   ![](assets/account-smart-lists-3.png)

1. Klicka på **Smart lista för konto**.

   ![](assets/account-smart-lists-4.png)

1. Ange ett namn och klicka på **Skapa** (Beskrivning och Etiketter är valfria).

   ![](assets/account-smart-lists-5.png)

Din smarta kontolista har skapats. Anvisningar om hur du definierar regler finns nedan.

## Regler för smarta kontouppsättningar {#account-smart-list-rules}

Smarta kontolistor fungerar på liknande sätt som vanliga smarta listor, med ett betydande undantag: behållare.

1. Om du vill definiera den smarta listan för ditt konto klickar du på fliken **Smart lista för konto**.

   ![](assets/account-smart-lists-6.png)

1. Välj önskade kontofilter. I det här exemplet väljer vi _Branschen är sjukvård_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >ICP-indikatordata som användes i din [kontoprofileringsrankning och justering](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) visas som anpassade kontoattribut som kan användas i din smarta kontolista. Dessa anpassade attributdata baseras på när kontoprofilmodellen skapades/uppdaterades.

1. Välj matchande personfilter. I det här exemplet väljer vi _Delstaten är Kalifornien_.

   ![](assets/account-smart-lists-9.png)

**VALFRITT STEG**: Här kommer behållare in. Om du väljer ytterligare ett Matchat personfilter kan du släppa det under det första, eller _i_ det, och skapa en behållare. I det här exemplet skapar vi en behållare genom att lägga till _Jobbtiteln är CFO_.

![](assets/account-smart-lists-10.png)

Så här ser behållaren ut.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Om du skapar en behållare med filter skapas en&quot;och&quot;-regel, vilket innebär att den bara returnerar alla resultat som kombineras. I det här exemplet har en vårdbransch som tillsammans med en annan i Kalifornien _och_ har någon som är listad som CFO. Om du inte vill använda behållare släpper du bara filtret nedanför/ovanför det befintliga.

Och det är allt! Se avsnittet nedan för att se hur du kan använda din smarta kontolista.

>[!TIP]
>
>Precis som med vanliga smarta listor kan du använda avancerad logik för att förfina resultaten ytterligare. Du behöver minst tre filter för att göra det, och i Smarta listor för konto är en behållare (oavsett hur många filter den innehåller) lika med ett filter.

## Åtgärder för smart lista för konto {#account-smart-list-actions}

På fliken Översikt i den smarta kontolistan finns några åtgärdsalternativ.

**Exportera**: Detta exporterar resultatet av din smarta kontolista som en CSV-fil.

**Klona**: Skapar en kopia av din smarta kontolista.

**Skicka till annonsnätverk**: Skickar listan till LinkedIn som en ny matchad publik.

Du kan också referera till din smarta kontolista i en smart kampanj/lista som är standard genom att använda filtret _Personmedlem i Smart lista_ för ditt konto.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Resultaten från Smart lista över personmedlemmar för konto visar alla personer i det/de identifierade kontot/kontona, inte bara personer som hittas via filter för matchad person i den smarta listan över konton.

>[!NOTE]
>
>**Definition**
>
>**Personmedlem i kontots smarta lista**: I det här fallet refererar ordet &quot;medlem&quot; till själva kontot, så &quot;personmedlem&quot; betyder de faktiska personerna (Marketo-poster) i dessa konton.
