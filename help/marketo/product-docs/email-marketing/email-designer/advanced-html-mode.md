---
solution: Marketo Engage
product: marketo
title: Lägg till anpassad CSS i e-postinnehållet
description: Lär dig hur du lägger till anpassad CSS i e-postinnehåll i e-postprogrammet för Designer. Stila dina e-postmeddelanden med anpassad kod i Marketo Engage.
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
source-git-commit: af89a1a1fd0246564d0904103f742230a096de04
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 2%

---

# Redigera e-postmallar med den avancerade HTML-redigeraren {#advanced-html-mode}

I avancerat HTML-läge kan du visa och redigera råkällkoden för e-postmallar direkt från Designer-gränssnittet i [!DNL Marketo Engage].

Med den här funktionen kan du infoga avancerade uttryck direkt i källan. När du växlar tillbaka till den visuella vyn (Skrivbord) återges innehållet på nytt så att du kan kontrollera hur det ser ut och fortsätta redigera i båda vyerna.

## Skyddsräcken {#guardrails}

När du använder den avancerade HTML-redigeraren skyddar följande skyddsutkast innehållets kompatibilitet och ställer in förväntningar.

* Den avancerade HTML-redigeraren **validerar inte** din kod. Syntaxfel och trasiga layouter kontrolleras inte. Granska innehållet noggrant innan du sparar.

* Framtida systemuppdateringar kan skriva över ändringar som du gör i standardkoden. **Ändringarna kanske inte kvarstår**.

* [!DNL Adobe] support **kan inte felsöka eller lösa**-problem som orsakas av anpassad kod och manuella ändringar. Spara en säkerhetskopia av innehållet ifall du skulle behöva återställa det.

* Du kan inte simulera innehåll i avancerad HTML-vy. Växla till skrivbordsvyn om du vill förhandsgranska innehållet.

* **Du kan inte spara** i den avancerade HTML-vyn för att säkerställa innehållskompatibiliteten. Växla tillbaka till skrivbordsvyn när du är redo att spara ändringarna.

## Använd avancerat HTML-läge {#access-html-mode}

Följ de här stegen för att öppna den avancerade HTML-redigeraren och redigera mallkällan.

1. Öppna eller [skapa en e-postmall](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template) i e-post-Designer.

1. Klicka på HTML-knappen i det övre högra hörnet på skärmen _Redigera e-postmall_.

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. Första gången du öppnar den avancerade HTML-redigeraren visas ett varningsmeddelande. Granska det genom att klicka på **[!UICONTROL OK]** när du är klar.

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >Den här varningen visas första gången du öppnar den avancerade HTML-redigeraren och återställer den varje månad.

1. Den avancerade HTML-redigeraren visas.

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. Lägg till önskade ändringar i e-postinnehållet.

   >[!WARNING]
   >
   >Se till att ange korrekt HTML- och CSS-kod eftersom det inte finns någon syntaxvalidering och Adobe Support kan inte hjälpa dig med redigeringen i HTML.

1. Simulering och sparande av innehåll är inte tillgängligt i avancerad HTML-vy av kompatibilitetsskäl. Växla tillbaka till skrivbordsvyn för att förhandsgranska innehållet och spara ändringarna.

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Dina redigeringar bevaras när du byter vy.
