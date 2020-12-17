---
unique-page-id: 2360309
description: Förstå arbetsytor och personpartitioner - Marketo Docs - Produktdokumentation
title: Arbetsytor och personpartitioner
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Arbetsytor och personpartitioner {#understanding-workspaces-and-person-partitions}

## Arbetsytor {#workspaces}

>[!CAUTION]
>
>Arbetsytor kan vara komplicerade att konfigurera.  Kontakta [Marketo Support](http://support.marketo.com/) för att ta reda på om de passar dig.

Arbetsytor är separata områden i Marketo som innehåller marknadsföringsresurser som program, landningssidor, e-post med mera. De kan användas av flera personer. Varje användare har tillgång till en eller flera arbetsytor.

>[!NOTE]
>
>**Exempel**
>
>En del orsaker till att du använder en arbetsyta:
>
>* Geografi: Marknadsföringsavdelningarna i Europa, Asien och Nordamerika får båda en arbetsyta
>* Affärsenhet: Snabbböcker, QuickBooks och TurboTax ger båda en arbetsyta

>
>
I båda fallen beror separationen på att marknadsföringsresurserna är helt olika. Om de delar marknadsföringsresurser kanske inte arbetsytorna är rätt verktyg för dig.

>[!NOTE]
>
>**Djupdykning**
>
>Lär dig hur du skapar [en ny arbetsyta](create-a-new-workspace.md).

## Dela mellan arbetsytor {#sharing-across-workspaces}

Så här delar du resurser mellan arbetsytor. Det fungerar på samma sätt för allt du vill dela. I det här exemplet visas segmenteringar.

>[!NOTE]
>
>Den överordnade mappen som innehåller dina resurser är den enda mappen som kan delas, inte de underordnade mapparna.

1. Skapa en ny mapp.

   ![](assets/one.png)

1. Namnge mappen som du vill dela.

   ![](assets/two.png)

1. Flytta de resurser som du vill dela till mappen.

   ![](assets/three.png)

1. Högerklicka på mappen och välj **Dela mapp**.

   ![](assets/four.png)

1. Markera arbetsytan/arbetsytorna som du vill dela mappen med och klicka på **Spara**. I dialogrutan Dela mapp visas endast arbetsytor som du har behörighet att visa.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >Ursprungsmappen har nu en liten grön pil, vilket anger att den delades. I den delade arbetsytan har mappen ett hänglås som anger att den är skrivskyddad.

Du kan dela dessa objekt mellan arbetsytor.

* E-postmallar
* Mallar för landningssidor
* Modeller
* Smarta kampanjer
* [Smarta listor](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmenteringar](share-segmentations-across-workspaces-and-partitions.md)
* Fragment

## Klona över arbetsytor {#cloning-across-workspaces}

För resurser som inte är mallar är det bäst att klona dem som lokala resurser i ett program.  Med rätt åtkomstnivå kan du dra och släppa resurserna på en annan arbetsyta:

* Program
* E-post
* Landningssidor
* Forms

>[!NOTE]
>
>När du klonar resurser som har mallar måste de mallarna delas med målarbetsytan.

## Flytta resurser till andra arbetsytor {#moving-assets-to-other-workspaces}

Om du vill flytta resurser till en ny arbetsyta placerar du dem i en mapp och drar mappen till den andra arbetsytan.

>[!NOTE]
>
>Du kan inte flytta ett program som innehåller medlemmar från en arbetsyta till en annan.

## Personpartitioner {#person-partitions}

Personpartitioner fungerar som separata databaser. Varje partition har sina egna personer som inte avduplicerar eller blandar med andra partitioner. Om du tror att du har ett affärsärende som kan göra det nödvändigt att ha dubblettposter med samma e-postadress kontaktar du [Marketo Support](http://support.marketo.com).

Du kan tilldela personpartitioner till [arbetsytor](create-a-new-workspace.md) i följande konfigurationer:

* en arbetsyta till en personpartition (1:1)
* en arbetsyta för många personpartitioner (1:x)
* många arbetsytor till en personpartition (x:1)

>[!NOTE]
>
>**Exempel**
>
>Orsaker till att du använder en personpartition:
>
>* Dina arbetsytor har inte bara olika resurser, de delar inga personer
>* Du vill ha dubbletter av andra affärsskäl

>



>[!CAUTION]
>
>Personpartitioner samverkar inte med varandra, så var försiktig när du konfigurerar dem.

>[!NOTE]
>
>**Djupdykning**
>
> Lär dig hur du [skapar en personpartition](create-a-person-partition.md).

