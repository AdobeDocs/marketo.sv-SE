---
unique-page-id: 1147108
description: Importera ett program - Marketo Docs - produktdokumentation
title: Importera ett program
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Importera ett program {#import-a-program}

Ett program kan importeras från en Marketo Engage-prenumeration till en annan. Du kan till exempel skapa ett program i en sandlåda och sedan importera det till din liveprenumeration. Du kan även importera ett fördefinierat program från [Marketo programbibliotek](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>Program som har smarta listor som innehåller utlösaren&quot;Anpassat objekt är uppdaterat&quot; kommer att göra att importen misslyckas. Ta bort den här utlösaren från alla smarta listor innan du följer stegen som beskrivs nedan.

## Importera ett program {#importing-a-program}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/import-a-program-1.png)

1. Klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL Import Program]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* Programimport är bara tillgängligt för användare som har roller med behörigheten Importera program aktiverad. Läs mer om att [hantera användarroller och behörigheter](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Om du vill ansluta ett sandlådekonto till din liveprenumeration kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Välj en Marketo **[!UICONTROL Subscription]** och ett program som ska importeras. Klicka på **[!UICONTROL Next]**.

   ![](assets/import-a-program-3.png)

1. Ange **[!UICONTROL Campaign Folder]** för det importerade programmet. Klicka på **[!UICONTROL Next]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Kontrollera att **[!UICONTROL Use default conflict]** regler är markerade. Konfliktregler behövs när du importerar program till en instans som har resurser med samma namn.

1. Välj önskad konfliktinformation och klicka på **[!UICONTROL Next]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Om du importerar ett program som använder anpassade flödessteg, eller smarta listregler som härleds från en Flow Step-tjänst, till en målinstans där det finns mer än en kompatibel tjänsteleverantör, uppmanas den importerande användaren att tilldela steg eller regler till rätt tjänsteleverantör i målinstansen.

1. Förhandsgranskningsinformation och **[!UICONTROL Import]** programmet.

   ![](assets/import-a-program-6.png)

Du får en bekräftelse via e-post när importen är klar.

>[!NOTE]
>
>Ni måste planera om importerade batchkampanjer och aktivera utlösarkampanjer. Systemet inaktiverar automatiskt kampanjscheman och utlöser kampanjer i det importerade programmet.

## Inverkan på externa Assets under programimporten {#impact-on-external-assets-during-program-imports}

Program använder externa resurser som e-postmallar, mallar för landningssidor, bilder, formulär, tokens och programtaggar. Du kan konfigurera hur mallarna och programtaggarna för landningssidor hanteras, och Marketo hanterar automatiskt resten.

**Mallar för e-post/landningssida:** Mallar för e-post/landningssida importeras till Design Studio. Du kan använda konfliktregler för att konfigurera beteendet när det finns en mall med samma namn. Med standardregeln läggs ett nummer till i en mall om det finns en mall med samma namn. Om du till exempel redan har en mall med namnet &quot;Standardmall&quot; får den nya namnet &quot;Standardmall - 1&quot;.

**Landningssidor/Forms:** Om det finns ett formulär eller en landningssida med samma namn i Design Studio importeras de fortfarande, men med en siffra tillagd till namnet (t.ex. landningssida - 1).

**Bilder:** Bilder som används av landningssidor importeras till designstudion om det inte finns någon bild med samma namn.

**Tokens:** Tokens som finns utanför ett program konverteras till lokala tokens under importprocessen.

>[!CAUTION]
>
>Bildtypen mina tokens stöds inte för programimporter. Om ett program som har bildtypen mina tokens importeras, kommer _no_-tokens att gå igenom.

**Programtaggar:** Du kan använda konfliktregler för att styra hur programtaggar som inte finns i målkontot behandlas. Om du använder standardregeln skapas programtaggarna, eller så kan du välja att ignorera taggarna.

>[!CAUTION]
>
>När du importerar ett program hoppas e-postmeddelanden/landningssidor som innehåller [dynamiskt innehåll](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} över.
