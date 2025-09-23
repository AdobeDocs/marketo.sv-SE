---
unique-page-id: 2360309
description: Förstå arbetsytor och personpartitioner - Marketo Docs - produktdokumentation
title: Arbetsytor och personpartitioner
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Arbetsytor och personpartitioner {#understanding-workspaces-and-person-partitions}

## Arbetsytor {#workspaces}

>[!CAUTION]
>
>Arbetsytor kan vara komplicerade att konfigurera. Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) för att ta reda på om de passar dig.

Arbetsytor är separata områden i Marketo som innehåller marknadsföringsresurser som program, landningssidor, e-post med mera. De kan användas av flera personer. Varje användare har tillgång till en eller flera arbetsytor.

>[!NOTE]
>
>**Exempel**
>
>En del orsaker till att du använder en arbetsyta:
>
>* Geografi: Marknadsföringsavdelningar i Europa, Asien och Nordamerika får båda en arbetsyta
>* Affärsenhet: [!DNL Quicken], [!DNL Quickbooks] och [!DNL TurboTax] får båda en arbetsyta
>
>I båda fallen beror separationen på att marknadsföringsresurserna är helt olika. Om de delar marknadsföringsresurser kanske inte arbetsytorna är rätt verktyg för dig.

>[!NOTE]
>
>Lär dig hur du skapar [en ny arbetsyta](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Dela mellan arbetsytor {#sharing-across-workspaces}

Så här delar du resurser mellan arbetsytor. Det fungerar på samma sätt för allt du vill dela. I det här exemplet visas segmenteringar.

>[!NOTE]
>
>Den överordnade mappen som innehåller dina resurser är den enda mappen som kan delas, inte de underordnade mapparna.

1. Klicka på **[!UICONTROL Database]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Högerklicka på segmenteringsmappen och klicka på **[!UICONTROL New Folder]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Namnge mappen och klicka på **[!UICONTROL Create]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Flytta de resurser som du vill dela till mappen.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Högerklicka på mappen och välj **[!UICONTROL Share Folder]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Markera den eller de arbetsytor som du vill dela mappen med och klicka på **[!UICONTROL Save]**. I dialogrutan Dela mapp visas endast arbetsytor som du har behörighet att visa.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >Ursprungsmappen har nu en liten grön pil, vilket anger att den delades. I den delade arbetsytan har mappen ett hänglås som anger att den är skrivskyddad.

Du kan dela dessa objekt mellan arbetsytorna.

* E-postmallar
* Mallar för landningssidor
* Models
* Smarta kampanjer
* [Smarta listor](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmenteringar](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Fragment

## Klona mellan arbetsytor {#cloning-across-workspaces}

För resurser som inte är mallar är det bäst att klona dem som lokala resurser i ett program. Med rätt åtkomstnivå kan du dra och släppa resurserna på en annan arbetsyta:

* Program
* E-post
* Landningssidor
* Forms

>[!IMPORTANT]
>
>Alla objekt som listas ovan kan klonas över arbetsytor, e-post, formulär och landningssidor _måste finnas i ett program_ vid kloningen.

>[!NOTE]
>
>När du klonar resurser som har mallar måste de mallarna delas med målarbetsytan.

## Flytta Assets till andra arbetsytor {#moving-assets-to-other-workspaces}

Om du vill flytta resurser till en ny arbetsyta placerar du dem i en mapp och drar mappen till den andra arbetsytan.

>[!NOTE]
>
>Du kan inte flytta ett program som innehåller medlemmar från en arbetsyta till en annan.

## Personpartitioner {#person-partitions}

Personpartitioner fungerar som separata databaser. Varje partition har sina egna personer som inte avduplicerar eller blandar med andra partitioner. Om du tror att du har ett affärsfall som kan göra det nödvändigt att ha dubblettposter med samma e-postadress kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

Du kan tilldela personpartitioner till [arbetsytor](create-a-new-workspace.md) i följande konfigurationer:

* en arbetsyta till en personpartition (1:1)
* en arbetsyta för många personpartitioner (1:x)
* många arbetsytor till en personpartition (x:1)

>[!NOTE]
>
>Orsaker till att du använder en personpartition:
>
>* Dina arbetsytor har inte bara olika resurser, de delar inga personer
>* Du vill ha dubbletter av andra affärsskäl

>[!CAUTION]
>
>Personpartitioner samverkar inte med varandra, så var försiktig när du konfigurerar dem.

>[!NOTE]
>
>Lär dig hur du [skapar en personpartition](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
