---
unique-page-id: 14352540
description: Förhindra självvisningar - Marketo Docs - Produktdokumentation
title: Förhindra självvisning
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Förhindrar självvisning {#preventing-self-views}

## Översikt {#overview}

Om du får en falsk positiv effekt på vyspårningen kan det leda till inkonsekvenser i rapporteringen. Detta inträffar ofta när användare av MSC av misstag anropar spårningspixeln från sin e-postklient (vi kallar detta en självgranskning). Nedan följer några tips om hur du kan minska och till och med ta bort självvisningar avsevärt.

## Webb (Outlook Web App och Gmail) {#web-outlook-web-app-and-gmail}

Sales Connect lagrar en cookie i webbläsaren för att förhindra att vyer spåras när du öppnar e-postmeddelanden från Outlook Web App och Gmail. Om du fortfarande får självvisningar rekommenderar vi att du gör följande:

* Kontrollera att du har aktiverat cookies på datorn.

* Om du använder en ny dator eller mobil enhet kontrollerar du att du har loggat in på webbprogrammet. Detta gör att vi kan känna igen din dator/enhet när vi går vidare.

## Skrivbord (Windows) {#desktop-windows}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i Outlook genom att inaktivera bilder som laddas ned automatiskt. Här nedan beskrivs hur du gör.

1. Klicka på **Arkiv** i menyraden i Outlook.

   ![](assets/win-1.png)

1. Klicka på **Alternativ**.

   ![](assets/win-2.png)

1. Klicka på **Trust Center** i dialogrutan Outlook-alternativ.

   ![](assets/win-3.png)

1. Under Microsoft Outlook Trust Center klickar du på **Trust Center Settings**.

   ![](assets/win-4.png)

1. Klicka på Automatisk hämtning på menyn till vänster och markera kryssrutan **Hämta inte bilder automatiskt i HTML-e-post eller RSS-alternativ**.

   ![](assets/win-5.png)

1. Klicka på **OK** i dialogrutan Säkerhetscenter.

   ![](assets/win-6.png)

1. Klicka på **OK** i dialogrutan Outlook-alternativ.

   ![](assets/win-6.png)

## Skrivbord (Mac) {#desktop-mac}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i Outlook genom att inaktivera bilder som laddas ned automatiskt. Här nedan beskrivs hur du gör.

1. I Outlook klickar du på **Outlook** i menyraden och väljer **Inställningar**.

   ![](assets/mac-1.png)

1. Välj **Läser** under E-post.

   ![](assets/mac-2.png)

1. Klicka på alternativknappen **Aldrig** under Säkerhet.

   ![](assets/mac-3.png)

