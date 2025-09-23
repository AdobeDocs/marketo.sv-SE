---
unique-page-id: 2950660
description: Skapa egna taggar - Marketo Docs - produktdokumentation
title: Skapa egna taggar
exl-id: f8efcbf5-7557-4cdf-b4e6-29d25b2fdd75
feature: Tags
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Skapa egna taggar {#create-custom-tags}

Taggar hjälper dig att organisera dina program medan kanaler hjälper dig att samla in data för rapportering.

>[!NOTE]
>
>Mer information finns i [Förstå taggar](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md).

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Skapa en ny taggtyp {#create-a-new-tag-type}

Så här skapar du en ny taggtyp:

1. Gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/create-custom-tags-1.png)

1. Klicka på **[!UICONTROL Tags]**.

   ![](assets/create-custom-tags-2.png)

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Tag Type]**.

   ![](assets/create-custom-tags-3.png)

1. Ange ett namn för taggtypen.

   ![](assets/create-custom-tags-4.png)

1. Ange önskat värde för taggtypen. Klicka på **[!UICONTROL Add Another]** om du vill ange ytterligare värden.

   ![](assets/create-custom-tags-5.png)

1. Välj vilken eller vilka programtyper taggen gäller för.

   ![](assets/create-custom-tags-6.png)

1. Bestäm om du vill att den här taggen ska användas för alla programtyper som visas.

   ![](assets/create-custom-tags-7.png)

   >[!NOTE]
   >
   >* Välj [!UICONTROL Required] om du vill att den här taggen ska läggas till när ett nytt program skapas.
   >* Om du tar bort en programtyp från listan [!UICONTROL Applies to] tas taggen och dess värden bort från alla befintliga program av den typen. Om du vill bevara befintliga taggvärden och göra den här taggen valfri att flytta framåt för _alla_ programtyper som visas, låter du kryssrutan Obligatorisk vara avmarkerad.

   >[!TIP]
   >
   >Om du vill göra en liknande tagg nödvändig för vissa programtyper men valfri för andra, måste du ställa in två separata taggar, som båda gäller för olika programtyper där den ena har [!UICONTROL Required] och den andra med [!UICONTROL Required] inte har valts.

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/create-custom-tags-8.png)
