---
unique-page-id: 1146897
description: Ta bort personer i en smart lista eller lista - Marketo Docs - produktdokumentation
title: Ta bort personer i en smart lista eller lista
exl-id: 192e79e6-d816-44e3-84c4-212cd73eb3ce
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Ta bort personer i en smart lista eller lista {#delete-people-in-a-smart-list-or-list}

Du kan snabbt och enkelt ta bort vissa/alla personer i en lista eller smart lista.

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Markera listan/den smarta listan som innehåller alla personer som du vill ta bort och gå till **Folk** -fliken.

   ![](assets/two-1.png)

   >[!CAUTION]
   >
   >När du tar bort en person tas de inte bara bort från listan, utan de tas helt bort från databasen.

1. Klicka **Markera alla**. Du kan också välja några poster manuellt med Ctrl/Cmd och klicka på.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Om resultatet sträcker sig över flera sidor klickar du på **Markera alla** markerar alla personer på alla sidor.

1. Om du vill ta bort alla personer från Marketo klickar du **Ta bort person**.

   ![](assets/four-1.png)

1. Ange **Ta bort från CRM** till **true** om du även vill ta bort posterna från CRM.

   ![](assets/five.png)

   >[!CAUTION]
   >
   >Om du tar bort från Marketo och CRM kommer du aldrig att kunna återställas i något av systemen. Människan och deras historia kommer att vara borta för evigt. Om du lägger till dem senare behandlas de som helt nya poster.

   >[!NOTE]
   >
   >Om din Marketo inte är knuten till din CRM är alternativet nedtonat, som i skärmbilden.

1. Klicka **Kör nu**.

   ![](assets/image2014-9-24-13-3a0-3a3.png)

1. Om du tar bort fler än 50 personer visas det här. Ange antalet personer som du vill ta bort, kontrollera **Kan inte ångra** och klicka sedan på **Ta bort**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Om du vill visa resultatet av massborttagningen klickar du på **Visa resultat** i popup-rutan Enstaka flödesåtgärd i skärmens övre högra hörn. Borttagningstiderna kan variera avsevärt beroende på olika faktorer.

   Det här är en bra funktion, var bara försiktig när du använder den!
