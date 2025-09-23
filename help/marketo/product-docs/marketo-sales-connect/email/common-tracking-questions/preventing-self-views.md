---
unique-page-id: 14352540
description: Förhindra självvisning - Marketo Docs - produktdokumentation
title: Förhindra självvisning
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Förhindra självvisning {#preventing-self-views}

## Översikt {#overview}

Om du får en falsk positiv effekt på vyspårningen kan det leda till inkonsekvenser i rapporteringen. Detta inträffar ofta när användare av MSC av misstag anropar spårningspixeln från sin e-postklient (vi kallar detta en självgranskning). Nedan följer några tips om hur du kan minska och till och med ta bort självvisningar avsevärt.

## Webb ([!DNL Outlook Web App] och Gmail) {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect] lagrar en cookie i webbläsaren för att förhindra att vyer spåras när du öppnar dina e-postmeddelanden från Outlook Web App och Gmail. Om du fortfarande får självvisningar rekommenderar vi att du gör följande:

* Kontrollera att du har aktiverat cookies på datorn.

* Om du använder en ny dator eller mobil enhet kontrollerar du att du har loggat in på webbprogrammet. Detta gör att vi kan känna igen din dator/enhet när vi går vidare.

## Skrivbord (Windows) {#desktop-windows}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i [!DNL Outlook] genom att inaktivera bilder som ska hämtas automatiskt. Här nedan beskrivs hur du gör.

1. I [!DNL Outlook] klickar du på **[!UICONTROL File]** i menyraden.

   ![](assets/win-1.png)

1. Klicka på **[!UICONTROL Options]**.

   ![](assets/win-2.png)

1. Klicka på [!DNL Outlook] i dialogrutan **[!UICONTROL Trust Center]** Alternativ.

   ![](assets/win-3.png)

1. Klicka på [!UICONTROL Microsoft Outlook Trust Center] under **[!UICONTROL Trust Center Settings]**.

   ![](assets/win-4.png)

1. Klicka på [!UICONTROL Automatic Download] på menyn till vänster och markera kryssrutan **[!UICONTROL Don't download pictures automatically in HTML email or RSS items]**.

   ![](assets/win-5.png)

1. Klicka på **[!UICONTROL OK]** i dialogrutan [!UICONTROL Trust Center].

   ![](assets/win-6.png)

1. Klicka på **[!UICONTROL OK]** i dialogrutan [!DNL Outlook] Alternativ.

   ![](assets/win-6.png)

## Skrivbord (Mac) {#desktop-mac}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i [!DNL Outlook] genom att inaktivera bilder som ska hämtas automatiskt. Här nedan beskrivs hur du gör.

1. I [!DNL Outlook] klickar du på **[!UICONTROL Outlook]** i menyraden och väljer **[!UICONTROL Preferences]**.

   ![](assets/mac-1.png)

1. Välj [!UICONTROL Email] under **[!UICONTROL Reading]**.

   ![](assets/mac-2.png)

1. Klicka på alternativknappen [!UICONTROL Security] under **[!UICONTROL Never]**.

   ![](assets/mac-3.png)
