---
description: Hur förhindrar jag självvisningar - Marketo Docs - produktdokumentation
title: Hur kan jag förhindra självvisningar?
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Hur förhindrar jag självvisningar? {#how-do-i-prevent-self-views}

Om du får en falsk positiv effekt på vyspårningen kan det leda till inkonsekvenser i rapporteringen. Detta inträffar ofta när användare av Marketo Sales av misstag anropar spårningspixeln från sin e-postklient (vi kallar detta en självgranskning). Nedan följer några tips om hur du kan minska och till och med ta bort självvisningar avsevärt.

## Webb (Outlook Web App och Gmail) {#web-outlook-web-app-and-gmail}

Marketo Sales lagrar en cookie i webbläsaren för att förhindra att vyer spåras när du öppnar e-postmeddelanden från Outlook Web App och Gmail. Om du fortfarande får självvisningar rekommenderar vi att du gör följande:

* Kontrollera att du har aktiverat cookies på datorn.

* Om du använder en ny dator eller mobil enhet kontrollerar du att du har loggat in på webbprogrammet. Detta gör att vi kan känna igen din dator/enhet när vi går vidare.

## Skrivbord (Windows) {#desktop-windows}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i Outlook genom att inaktivera bilder som laddas ned automatiskt. Här nedan beskrivs hur du gör.

1. Klicka på **Arkiv** i menyraden i Outlook.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Klicka på **Alternativ**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Klicka på **Trust Center** i dialogrutan Outlook-alternativ.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Klicka på **Inställningar för Trust Center** under Microsoft Outlook Trust Center.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Klicka på Automatisk hämtning på menyn till vänster och markera kryssrutan **Hämta inte bilder automatiskt i HTML-e-post eller RSS-objekt** .

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Klicka på **OK** i dialogrutan Säkerhetscenter.

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Klicka på **OK** i dialogrutan Outlook-alternativ.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Skrivbord (Mac) {#desktop-mac}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i Outlook genom att inaktivera bilder som laddas ned automatiskt. Här nedan beskrivs hur du gör.

1. I Outlook klickar du på **Outlook** i menyraden och väljer **Inställningar**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Välj **Läser** under E-post.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Klicka på alternativknappen **Aldrig** under Säkerhet.

   ![](assets/how-do-i-prevent-self-views-10.png)
