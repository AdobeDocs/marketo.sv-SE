---
description: Hur förhindrar jag självvisningar - Marketo Docs - produktdokumentation
title: Hur kan jag förhindra självvisningar?
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Hur förhindrar jag självvisningar? {#how-do-i-prevent-self-views}

Om du får en falsk positiv effekt på vyspårningen kan det leda till inkonsekvenser i rapporteringen. Detta inträffar ofta när användare av [!DNL Marketo Sales] av misstag anropar spårningspixeln från sin e-postklient (vi kallar detta en självgranskning). Nedan följer några tips om hur du kan minska och till och med ta bort självvisningar avsevärt.

## Webb ([!DNL Outlook] webbapp och Gmail) {#web-outlook-web-app-and-gmail}

[!DNL Marketo Sales] lagrar en cookie i din webbläsare för att förhindra att vyer spåras när du öppnar dina e-postmeddelanden från [!DNL Outlook] Web App och Gmail. Om du fortfarande får självvisningar rekommenderar vi att du gör följande:

* Kontrollera att du har aktiverat cookies på datorn.

* Om du använder en ny dator eller mobil enhet kontrollerar du att du har loggat in på webbprogrammet. Detta gör att vi kan känna igen din dator/enhet när vi går vidare.

## Skrivbord (Windows) {#desktop-windows}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i [!DNL Outlook] genom att inaktivera bilder som ska hämtas automatiskt. Här nedan beskrivs hur du gör.

1. Klicka på **[!UICONTROL File]** i menyraden i Outlook.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Klicka på **[!UICONTROL Options]**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Klicka på [!DNL Outlook] i dialogrutan **[!UICONTROL Trust Center]** Alternativ.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Klicka på [!DNL Outlook] under Microsoft **[!UICONTROL Trust Center Settings]** Trust Center.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Klicka på [!UICONTROL Automatic Download] på menyn till vänster och markera kryssrutan **[!UICONTROL Don't download pictures automatically in HTML email or RSS items]**.

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Klicka på **[!UICONTROL OK]** i dialogrutan [!UICONTROL Trust Center].

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Klicka på **[!UICONTROL OK]** i dialogrutan [!DNL Outlook] Alternativ.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Skrivbord (Mac) {#desktop-mac}

Vyer spåras genom att en liten osynlig bildpixel hämtas till din e-postklient. Du kan avsevärt minska antalet självvisningar i [!DNL Outlook] genom att inaktivera bilder som ska hämtas automatiskt. Här nedan beskrivs hur du gör.

1. I [!DNL Outlook] klickar du på **[!UICONTROL Outlook]** i menyraden och väljer **[!UICONTROL Preferences]**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Välj [!UICONTROL Email] under **[!UICONTROL Reading]**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Klicka på alternativknappen [!UICONTROL Security] under **[!UICONTROL Never]**.

   ![](assets/how-do-i-prevent-self-views-10.png)
