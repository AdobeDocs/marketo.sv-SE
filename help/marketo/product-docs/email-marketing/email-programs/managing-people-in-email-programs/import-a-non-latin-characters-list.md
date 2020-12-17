---
unique-page-id: 5472678
description: Importera en icke-latinsk teckenlista - Marketo Docs - Produktdokumentation
title: Importera en icke-latinsk teckenlista
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Importera en icke-latinsk teckenlista {#import-a-non-latin-characters-list}

Försöker du importera en fil som inte är på engelska? Listan ser perfekt ut när du öppnar den med Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Men när du importerar det till Marketo kanske du ser att de icke-engelska tecknen inte plockas upp korrekt.

![](assets/image2015-2-10-9-3a35-3a49.png)

Det beror på att filen inte har sparats korrekt för Marketo för att alla icke-latinska tecken ska kännas igen. Den goda nyheten är att du kan följa några enkla steg för att åtgärda det.

1. Välj **Spara som..** från menyn **Arkiv** i Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Välj **UTF-16 Unicode-text (.txt)** som **Format**-alternativ. Detta kodar filen så som Marketo kan visa den.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo har också stöd för UTF-8, Shift-JIS eller EUC-JP.

1. Excel sparar den nya filen som en textfil med tillägget .txt. Men det konverterar också alla kommatecken i filen till flikar. Vi måste ändra tillbaka den.

   >[!TIP]
   >
   >Du kan öppna textfilen med **Anteckningar** om du använder Windows eller **TextEdit** om du använder en Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Välj en flik i dokumentet och kopiera den.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Välj **Sök och ersätt...** från menyn **Redigera**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Motsvarande åtgärd för Windows-användare är: **Redigera > Ersätt..**

1. Klistra in fliken som du kopierade i steg 4 i den första rutan (som ska ersättas) och skriv in ett kommatecken i den andra rutan (ersätt med). Klicka sedan på **Alla**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Och voila, alla kommatecken är tillbaka och vi är redo att rulla.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importera den nya filen till Marketo så ska informationen visas korrekt den här gången.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Alla datum-/tidfält som importeras behandlas som centraltid. Om du har datum-/tidsfält i en annan tidszon kan du använda en Excel-formel för att omvandla den till Central Time (USA/Chicago).

Vi vet att det här är underligt, men det fungerar. Glad import!