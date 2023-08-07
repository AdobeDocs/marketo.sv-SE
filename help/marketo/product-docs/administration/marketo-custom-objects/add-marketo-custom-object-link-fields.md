---
unique-page-id: 10097613
description: Lägg till Marketo anpassade objektlänkfält - Marketo Docs - produktdokumentation
title: Lägg till Marketo anpassade objektlänkfält
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 1dbe820e126f92ce5820e38414925605372a4b09
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Lägg till Marketo anpassade objektlänkfält {#add-marketo-custom-object-link-fields}

När du skapar anpassade objekt måste du tillhandahålla länkfält för att kunna koppla den anpassade objektposten till rätt överordnade post.

* Om du vill ha en anpassad struktur som är en-till-många använder du länkfältet i det anpassade objektet för att ansluta det till en person eller ett företag.
* För många-till-många-strukturer använder du två länkfält som är anslutna från ett separat skapat mellanliggande objekt (som också är en typ av anpassat objekt). En länk ansluter till personer eller företag i din databas och den andra ansluter till det anpassade objektet. I det här fallet finns inte länkfältet i det anpassade objektet.

>[!IMPORTANT]
>
>Marketo Engage har bara stöd för ett enda kantobjekt för varje bryggobjekt i relationen många till många. I exemplet nedan kan varje registrering bara länka till en enda kurs. Det kan dock finnas många bryggobjekt för varje edge-objekt, precis som det finns många elevregistreringar för varje kurs (många-till-ett-förhållande). Om du har strukturerat anpassade objektdata så att det finns mer än en Edge-objektspost för varje Bridge-objektpost (En-till-Många eller Många-till-Många), kan du skapa flera Bridge-objektposter som var och en refererar till en enda Edge-objektpost som representerar dessa data i Marketo.

## Skapa ett länkfält för en 1:N-struktur {#create-a-link-field-for-a-one-to-many-structure}

Så här skapar du ett länkfält i ett anpassat objekt för en 1:N-struktur.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Markera det anpassade objektet i listan.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. I **[!UICONTROL Fields]** flik, klicka **[!UICONTROL New Field]**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Namnge länkfältet och lägg till ett valfritt [!UICONTROL Description]. Se till att du väljer [!UICONTROL Link] datatyp.

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Du kan inte gå tillbaka och skapa, redigera eller ta bort en [!UICONTROL Link] eller [!UICONTROL Dedupe Field] när det anpassade objektet har godkänts.

1. Välj om [!UICONTROL Link Object] är för [!UICONTROL lead] (person) eller en [!UICONTROL company].

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Om du väljer [!UICONTROL lead]visas ID, e-postadress och eventuella anpassade fält i listan.
   >
   >Om du väljer [!UICONTROL company]visas ID och anpassade fält i listan.

1. Välj [!UICONTROL Link Field] som du vill ansluta till som överordnad till det nya fältet.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >Endast strängfälttyper stöds i länkfältet.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Skapa ett länkfält för en många-till-många-struktur {#create-a-link-field-for-a-many-to-many-structure}

Så här skapar du ett länkfält i ett mellanliggande objekt som kan användas i en många-till-många-struktur.

>[!PREREQUISITES]
>
>Du måste redan ha skapat mellanliggande objekt och eventuella anpassade objekt som du vill länka det till.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Markera det mellanliggande objekt som du vill lägga till fältet i.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. I **[!UICONTROL Fields]** flik, klicka **[!UICONTROL New Field]**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Du måste skapa två länkfält. Skapa dem en åt gången. Ge först fältet ett namn för medlemmarna i databaslistan (till exempel leadID). Lägg till ett valfritt [!UICONTROL Description]. Se till att du väljer [!UICONTROL link] [!UICONTROL Data Type].

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Du kan inte gå tillbaka och skapa, redigera eller ta bort en [!UICONTROL Link] eller [!UICONTROL Dedupe Field] när det anpassade objektet har godkänts.

1. Välj [!UICONTROL Link Object] från databasen, i det här fallet [!UICONTROL Lead].

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Välj [!UICONTROL Link Field] du vill ansluta till, i det här fallet, [!UICONTROL Id].

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >Endast strängfälttyper stöds i [!UICONTROL Link Field].

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Upprepa den här processen för den andra länken till ditt anpassade objekt, i det här exemplet, kursID. The [!UICONTROL Link Object] namnet ska vara kurs, och [!UICONTROL Link Field] blir kursID. Eftersom du redan har skapat och godkänt det anpassade kursobjektet är dessa val tillgängliga i listrutorna.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Skapa andra fält som du vill använda i mellanliggande objekt, till exempel enrollmentID eller grad.

## Använda anpassade objekt {#using-custom-objects}

Nästa steg är att använda dessa anpassade objekt i filter i smarta kampanjer. Med många-till-många-relationer kan du markera flera personer/företag och flera anpassade objekt. I exemplet nedan listas alla i din databas som uppfyller dessa villkor. Fältet för lärarnamn kommer från det anpassade kursobjektet och registreringsklassen kommer från det mellanliggande objektet.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Lägg till anpassade Marketo-objektfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Redigera och ta bort ett anpassat Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Redigera och ta bort anpassade Marketo-objektfält](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
