---
unique-page-id: 1146997
description: Använd en datumtoken i ett vänteflödessteg - Marketo Docs - Produktdokumentation
title: Använd en datumtoken i ett vänteflödessteg
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Använd en datumtoken i ett vänteflödessteg {#use-a-date-token-in-a-wait-flow-step}

Du kan använda steget Väntflöde för att pausa en persons resa genom en smart kampanj tills ett visst datum som använder en datumtoken. Du kan också ändra slutdatumet med ett antal dagar.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Detta gäller endast utlösande kampanjer. Du kan inte använda den här funktionen i gruppkampanjer.

1. Dra över steget **Vänta** i det smarta **kampanjflödet** .

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Klicka på kugghjulsikonen till höger.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. I listrutan **Typ** väljer du **Datumtoken**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Välj en datumtoken som anger när vänsteget ska avslutas:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Markera kryssrutan om du vill vänta till nästa årsdag för datumet som infaller under det aktuella eller nästa kalenderår.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Använd det här alternativet för datumtoken som refererar till tidigare datum, t.ex. en födelsedag eller ett kontraktstartdatum.

1. Du kan också ändra slutdatumet med ett visst antal dagar.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Du kan också ange antalet dagar med hjälp av ett `{{lead.` - eller `{{company.` token som representerar ett heltalsfält eller en `{{my.` token av taltyp.

1. Klicka på Spara.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >* [Använd en varaktighet i ett vänteflödessteg](use-a-duration-in-a-wait-flow-step.md)
   >* [Använd ett specifikt datum i ett vänteflödessteg](use-a-specific-date-in-a-wait-flow-step.md)


