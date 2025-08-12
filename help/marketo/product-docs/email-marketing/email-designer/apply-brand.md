---
solution: Marketo Engage
product: marketo
title: RUBRIK
description: Lär dig hur du kan effektivisera e-postgenereringen med återanvändbara teman och moduler, vilket ger en enhetlig design och effektivitet.
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 1cfb28f47ba3c168292b298e1fc7ab2ff638b412
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Använd teman i ditt e-postinnehåll {#apply-email-themes}

>[!AVAILABILITY]
>
>Funktionen finns för närvarande i betaversion och är endast tillgänglig för betatestare. Kontakta din Adobe-representant om du vill delta i betaprogrammet.

Med teman kan icke-tekniska användare skapa återanvändbart innehåll som passar ett visst varumärke och designspråk genom att lägga till anpassad formatering ovanpå standardmallarna <!-- to achieve brand specific results-->.

Den här funktionen gör att marknadsförarna kan använda visuellt tilltalande, varumärkesenhetliga e-postmeddelanden snabbare och enklare, samtidigt som de erbjuder avancerade anpassningsalternativ för unika designbehov.

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## Skyddsritningar och begränsningar {#themes-guardrails}

* När du skapar ett e-postmeddelande från grunden kan du välja att börja bygga ditt innehåll med ett tema för att snabbt tillämpa en specifik formatering som passar ert varumärke och er design.

  Om du väljer läget _Manuell formatering_ kan du inte använda några teman om du inte återställer e-postmeddelandet.

* [Fragment](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) är inte korskompatibla mellan lägena _Använd teman_ och _Manuell formatering_.

  Om du vill kunna använda ett fragment i ett innehåll där ett tema används måste det här fragmentet skapas i _Använd teman_ .

* Om du använder innehåll som skapats i HTML är du i [kompatibilitetsläge](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) och kan inte använda teman för det här innehållet.

  Om du vill utnyttja alla funktioner i e-post-Designer, inklusive teman, måste du antingen skapa nytt innehåll i _Använd teman_ eller konvertera [importerat HTML-innehåll](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html).

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## Skapa ett tema {#create-and-edit-themes}

Följ stegen nedan för att definiera ett tema som du kan använda i ditt framtida e-postinnehåll.

1. Skapa en ny [e-postmall](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template) för att komma igång.

1. Välj alternativet **[!UICONTROL Create or edit themes]**.

   `![](assets/theme-create.png)`

1. Du kan antingen välja standardtemat eller använda en Adobe-mall eller en anpassad mall. I det här exemplet väljer du standardtemat och klickar på **[!UICONTROL Create]**.

   `![](assets/theme-select.png)`

1. Börja att definiera ditt tema på fliken **[!UICONTROL General settings]** genom att ge det ett specifikt namn för ditt varumärke. Du kan justera standardbredden för dina e-postmeddelanden och även exportera det aktuella temat för att dela det över sandlådor.

   `<!--![](assets/theme-general-settings.png)-->`

1. Använd listen till höger för att navigera mellan de olika flikarna och uppdatera designinställningarna.

   `![](assets/theme-right-pane.png)`

1. Från fliken **[!UICONTROL Colors]**:

   * Använd knappen **[!UICONTROL Edit]** för att konfigurera en **[!UICONTROL Color palette]** med standardfärger för ditt varumärke. Välj en **[!UICONTROL Preset]** om du snabbt vill skapa ett färgschema eller justera varje färg i temat individuellt. Du kan också använda en kombination av båda.

     `![](assets/theme-colors.gif)`

   * Klicka på **[!UICONTROL Add variant]** om du vill skapa flera färgvarianter, till exempel ljust och mörkt läge, där varje variant har sina egna färgpalett- och nyanskontroller.

     `![](assets/theme-colors-variant.png)`

   * Klicka på redigeringsikonen för varje variant för att redigera ett enskilt element. Du kan använda standardpaletten som du har skapat eller andra anpassade färger.

     `![](assets/theme-colors-edit-variant.gif)`

1. I **[!UICONTROL Text settings]** kan du ange det globala teckensnitt som du vill använda för hela temat. Du kan också redigera varje rubrik- och stycketyp för att justera teckensnitt, storlek, format och så vidare.

   `![](assets/theme-text.png)`

1. På fliken **[!UICONTROL Spacing]** väljer du ett enskilt element i listan för att det ska vara tillräckligt stort mellan de olika komponenterna.

   `<!--![](assets/theme-spacing.png)-->`

1. Med de andra flikarna till höger kan du hantera varje knappelement, avgränsare, extra bildformatering och mellanrum för stödrasterlayout separat för det här temat.

   `<!--![](assets/theme-buttons.png)-->`

1. Klicka på **[!UICONTROL Save]** om du vill lagra det här temat för framtida bruk.

## Använda teman i ett e-postmeddelande {#apply-themes}

Följ stegen nedan om du vill använda standardteman eller anpassade formatteman i ett e-postmeddelande.

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. Du kan välja någon av följande åtgärder:

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >Om du väljer läget _Manuell formatering_ kan du inte använda några teman om du inte återställer e-postmeddelandet.
     >
     >Om du vill använda ett [fragment](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) i _Använd teman_ måste det här fragmentet ha skapats med läget _Använd teman_.

1. Klicka på knappen **[!UICONTROL Themes]** till höger i e-post-Designer. Standardtemat eller mallens tema visas. Du kan växla mellan de två färgvarianterna för det här temat.

   `![](assets/theme-default-hero.png)`

1. Klicka på pilen bredvid det tema som används för närvarande. Listan med tillgängliga anpassade teman och Adobe-teman visas.

   `![](assets/theme-hero-change.png)`

1. Klicka på **[!UICONTROL Custom themes]** och välj det tema som du skapade.

   `![](assets/theme-select-custom.png)`

1. Klicka utanför listrutan. Det nya anpassade temat använder automatiskt sina format på alla e-postkomponenter. Du kan växla mellan de två färgvarianterna.

1. När en komponent är markerad kan du fortfarande låsa upp dess stil med den dedikerade ikonen.

   `![](assets/theme-unlock-style.png)`

Du kan växla teman när som helst. E-postinnehållet ändras inte, men formaten uppdateras för att återspegla det nya temat.

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->
