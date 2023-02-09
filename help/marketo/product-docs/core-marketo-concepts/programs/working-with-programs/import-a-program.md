---
unique-page-id: 1147108
description: Importera ett program - Marketo Docs - produktdokumentation
title: Importera ett program
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
source-git-commit: adff42d54d7953c9ec72e4d736ce0153502be960
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Importera ett program {#import-a-program}

Ett program kan importeras från en Marketo-prenumeration till en annan. Du kan till exempel skapa ett program i en sandlåda och sedan importera det till din liveprenumeration. Du kan även importera ett färdigbyggt program från Marketo Program Library.

## Importera ett program {#importing-a-program}

1. Gå till **Marknadsföringsaktiviteter.**

   ![](assets/import-a-program-1.png)

1. Klicka **Nytt** nedrullningsbar meny. Välj **Importprogram**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >Programimport är bara tillgängligt för användare som har roller med behörigheten Importera program aktiverad. Läs mer om [hantera användarroller och behörigheter](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Om du vill ansluta ett sandlådekonto till din liveprenumeration kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Välj en Marketo **Prenumeration** och ett program att importera. Klicka **Nästa**.

   ![](assets/import-a-program-3.png)

1. Ange en **Campaign-mapp** för det importerade programmet. Klicka **Nästa.**

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Se till att **Använd standardkonflikt** regler är markerade. Konfliktregler behövs när du importerar program till en instans som har resurser med samma namn.

1. Välj önskad konfliktinformation och klicka på **Nästa**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Om du importerar ett program som använder anpassade flödessteg, eller smarta listregler som härleds från en Flow Step-tjänst, till en målinstans där det finns mer än en kompatibel tjänsteleverantör, uppmanas den importerande användaren att tilldela steg eller regler till rätt tjänsteleverantör i målinstansen.

1. Förhandsgranska information och **Importera** programmet.

   ![](assets/import-a-program-6.png)

Du får en bekräftelse via e-post när importen är klar.

>[!NOTE]
>
>Ni måste planera om importerade batchkampanjer och aktivera utlösarkampanjer. Systemet inaktiverar automatiskt kampanjscheman och utlöser kampanjer i det importerade programmet.

## Inverkan på externa resurser under programimporten {#impact-on-external-assets-during-program-imports}

Program använder externa resurser som e-postmallar, mallar för landningssidor, bilder, formulär, tokens och programtaggar. Du kan konfigurera hur landningssidmallar och programtaggar hanteras, och Marketo hanterar automatiskt resten.

**Mallar för e-post/landningssida:** Mallar för e-post/landningssida importeras till Design Studio. Du kan använda konfliktregler för att konfigurera beteendet när det finns en mall med samma namn. Med standardregeln läggs ett nummer till i en mall om det finns en mall med samma namn. Om du till exempel redan har en mall med namnet &quot;Standardmall&quot; får den nya namnet &quot;Standardmall - 1&quot;.

**Landningssidor/Forms:** Om det finns ett formulär eller en landningssida med samma namn i Design Studio importeras de fortfarande, men med en siffra efter namn (t.ex.: Landningssida - 1).

**Bilder:** Bilder som används av landningssidor importeras till designstudion om det inte finns någon bild med samma namn.

**Tokens:** Token som finns utanför ett program konverteras till lokala tokens under importprocessen.

>[!CAUTION]
>
>Bildtypen mina tokens stöds inte för programimporter. Om ett program som har bildtypen mina tokens importeras, **no** Token kommer fram.

**Programtaggar:** Du kan använda konfliktregler för att styra hur programtaggar som inte finns i destinationskontot behandlas. Om du använder standardregeln skapas programtaggarna, eller så kan du välja att ignorera taggarna.

>[!CAUTION]
>
>När du importerar ett program skickas e-postmeddelanden eller landningssidor som innehåller [dynamiskt innehåll](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) kommer att hoppas över.
