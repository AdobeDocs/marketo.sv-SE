---
unique-page-id: 2360287
description: Skapa ett anpassat fält i Marketo - Marketo Docs - Produktdokumentation
title: Skapa ett anpassat fält i Marketo
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# Skapa ett anpassat fält i Marketo {#create-a-custom-field-in-marketo}

Om du behöver ett nytt anpassat fält i Marketo för att lagra/hämta data, så här skapar du ett.

1. Gå till Admin och klicka på Fälthantering.

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >Om du vill att fälten ska synkroniseras med CRM skapar du dem i CRM så skapas de automatiskt i Marketo.

1. Klicka på Nytt anpassat fält.

   ![](assets/two.png)

1. Välj fälttyp. Detta ändrar hur det återges i smarta listor och formulär i Marketo.

   >[!TIP]
   >
   >Läs ordlistan för [anpassade fälttyper](custom-field-type-glossary.md).

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. Ange namnet som du vill att det ska visas i Marketo. API-namnet genereras automatiskt. Du kan ändra den, men du kan inte byta namn på den när den har angetts. Klicka på Skapa när du är klar.

>[!CAUTION]
>
>Fältnamn får inte börja med följande tecken: **. &amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>API-namnet används av SOAP API och andra serverdelsprocesser.

Du kan nu använda det här anpassade fältet i formulär, flödessteg och smarta listor.