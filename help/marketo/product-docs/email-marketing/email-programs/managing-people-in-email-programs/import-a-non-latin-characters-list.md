---
unique-page-id: 5472678
description: Importera en icke-latinsk teckenlista - Marketo Docs - produktdokumentation
title: Importera en icke-latinsk teckenlista
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Importera en icke-latinsk teckenlista {#import-a-non-latin-characters-list}

Försöker du importera en fil som inte är på engelska? Listan ser perfekt ut när du öppnar den med Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Men när du importerar den till Marketo kanske du ser att de tecken som inte är engelska inte plockas upp korrekt.

![](assets/image2015-2-10-9-3a35-3a49.png)

Detta beror på att filen inte har sparats på rätt sätt så att Marketo kan identifiera alla tecken som inte är latinska. Den goda nyheten är att du kan följa några enkla steg för att åtgärda det.

1. Välj **[!UICONTROL Save As]..** på menyn **[!UICONTROL File]** i Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Välj **[!UICONTROL UTF-16 Unicode Text (.txt)]** som **[!UICONTROL Format]**-alternativ. Då kodas filen som den visas i Marketo.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo har också stöd för UTF-8, Shift-JIS eller EUC-JP.

1. Excel sparar den nya filen som en textfil med tillägget .txt. Men det konverterar också alla kommatecken i filen till flikar. Vi måste ändra tillbaka den.

   >[!TIP]
   >
   >Du kan öppna textfilen med **[!DNL Notepad]** om du använder Windows eller **[!DNL TextEdit]** om du använder en Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Välj en flik i dokumentet och kopiera den.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Välj **[!UICONTROL Find and Replace]..** på menyn **[!UICONTROL Edit]**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Motsvarande åtgärd för Windows-användare är: **[!UICONTROL Edit]> [!UICONTROL Replace]..**

1. Klistra in fliken som du kopierade i steg 4 i den första rutan (som ska ersättas) och skriv in ett kommatecken i den andra rutan (ersätt med). Klicka sedan på **[!UICONTROL All]**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Och voila, alla kommatecken är tillbaka och vi är redo att rulla.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importera den nya filen till Marketo så bör informationen visas korrekt den här gången.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Alla datum-/tidfält som importeras behandlas som centraltid. Om du har datum-/tidsfält i en annan tidszon kan du använda en Excel-formel för att omvandla den till Central Time (USA/Chicago).

Vi vet att det här är underligt, men det fungerar. Glad import!
