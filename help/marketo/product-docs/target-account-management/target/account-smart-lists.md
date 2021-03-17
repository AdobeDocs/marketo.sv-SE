---
unique-page-id: 11378814
description: Smarta kontolistor - Marketo Docs - Produktdokumentation
title: Smarta kontouppsättningar
translation-type: tm+mt
source-git-commit: 96d6cc030ecd9d1da844fe27e1c6f62bbd181d62
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Smarta kontolistor {#account-smart-lists}

Så här identifierar du snabbt och korrekt dina värdefulla konton.

>[!NOTE]
>
>Den här funktionen finns i en Open Beta och är tillgänglig för alla som har både TAM och Marketo Next-Gen aktiverat. Kontakta din CSM om du vill delta i betaversionen.

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

1. Klicka på fliken **Smart lista för konto** för att definiera din smarta lista för ditt konto.

   ![](assets/account-smart-lists-6.png)

1. Välj önskade kontofilter. I det här exemplet väljer vi _Branschen är Healthcare_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. Välj matchande personfilter. I det här exemplet väljer vi _Delstaten är Kalifornien_.

   ![](assets/account-smart-lists-9.png)

**Valfritt steg**: Här kommer containrar in. Om du väljer ytterligare ett Matchat personfilter kan du släppa det under det första, eller _i_, och skapa en behållare. I det här exemplet skapar vi en behållare genom att lägga till _Jobbtitel är CFO_.

![](assets/account-smart-lists-10.png)

Så här ser behållaren ut.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>När du skapar en behållare med filter skapas en&quot;och&quot;-regel, vilket innebär att den bara returnerar alla resultat som kombineras. I det här exemplet står för en vårdbransch och finns i Kalifornien _och_ med någon som är listad som CFO. Om du inte vill använda behållare släpper du bara filtret nedanför/ovanför det befintliga.

Och det är allt! Läs igenom avsnittet nedan för att se hur du kan använda Smart lista för ditt konto.

>[!TIP]
>
>Precis som med vanliga smarta listor kan du använda avancerad logik för att förfina dina resultat ytterligare. Du behöver minst tre filter för att göra det, och i Smarta listor för konto är en behållare (oavsett hur många filter den innehåller) lika med ett filter.

## Åtgärder för smart lista för konto {#account-smart-list-actions}

På fliken Översikt i din smarta kontolista finns några åtgärdsalternativ.

**Exportera**: Resultatet av din smarta lista över konton exporteras som en CSV-fil.

**Klona**: Skapar en kopia av din smarta kontolista.

**Skicka till annonsnätverk**: Skickar listan till LinkedIn som en ny Matchad målgrupp.

Du kan också referera till din smarta kontolista i en standardlista för smarta kampanjer/listor genom att använda filtret _Personer som är medlem i den smarta kontolistan_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Resultaten av Smart lista över personmedlemmar för konto visar alla personer i de identifierade kontona, inte bara personer som hittas via filtrering av matchad person i den smarta listan över konton.

>[!NOTE]
>
>**Definition**
>
>**Smart lista över** personmedlemmar för konto: I det här fallet avser ordet&quot;medlem&quot; själva kontot, så&quot;personmedlem&quot; avser de faktiska personerna (Marketo-posterna) i dessa konton.
