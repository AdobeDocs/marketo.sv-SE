---
unique-page-id: 2359646
description: Konfigurera progressiv formulärprofilering - Marketo Docs - Produktdokumentation
title: Konfigurera progressiv profilering av formulär
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Konfigurera progressiv profilering av formulär {#configure-form-progressive-profiling}

Korta formulär är bra. När någon kommer tillbaka till ett formulär kan du presentera nya fält och progressivt fylla i besökarens profil. Så här gör du.

>[!NOTE]
>
>För att den här funktionen ska fungera på rätt sätt måste formulärförifyllning vara aktiverat för synliga fält och [inaktiverat](http://docs.marketo.com/display/DOCS/Disable+Pre-fill+for+a+Form+Field) för dolda fält.

1. Gå till **Marknadsföringsaktiviteter** och **aktiviteter**.

   ![](assets/ma-1.png)

1. Markera formuläret och klicka på **Redigera** **formulär**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Klicka på **Inställningar** under **Formulärinställningar******.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Ange **Progressiv** **profilering** som **aktiverad**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Nu ska vi konfigurera det. Gå till **Fältinformation** **Information**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)
Dra och släpp alla fält som ingår i den progressiva profiluppsättningen.
   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. När du har flyttat alla fält bör det se ut ungefär så här:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Fälten utanför rutan **Progressiv** **profilering** visas alltid i formuläret, även om de är ifyllda.

1. Markera rutan **Progressiv** **profilering** .

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Var försiktig när du använder obligatoriska fält i Progressiv profilering. Dessa fält kan fortfarande lämnas tomma om besökaren anger en ny e-postadress (som skulle skapa en ny person) efter att tidigare ha skickat data för de andra fälten, eftersom de då skulle ignoreras i det senaste formuläret.

1. Välj nu hur många tomma fält du vill att personer ska se i rutan **Progressiv** **profilering** vid varje given tidpunkt.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >**Exempel**
   >
   >
   >Om du väljer **Antal** **för** **tomma** **fält** som 1 visas följande första gången de ser det här formuläret:
   >
   >    
   >    
   >    * Förnamn (tomt)
   >    * Efternamn (tomt)
   >    * E-postadress (tom)
   >    * Telefonnummer (tomt)

   >    
   >    
   >Förutsatt att de fyller i alla fält, andra gången de besöker, kommer de att se:
   >
   >    
   >    
   >    * Förnamn (förifyllt)
   >    * Efternamn (förifyllt)
   >    * E-postadress (förifylld)
   >    * Mobiltelefonnummer (tomt)

   >    
   >    
   >Förutsatt att de fyller i mobiltelefonnumret kommer de tredje gången de besöker att se:
   >
   >    
   >    
   >    * Förnamn (förifyllt)
   >    * Efternamn (förifyllt)
   >    * E-postadress (förifylld)
   >    * Land (tomt)


1. Klicka på **Slutför**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Klicka på **Godkänn och stäng**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Snyggt jobb! Det arbete du just gjorde lönar sig.

Experimentera med den här funktionen och se till att testa den. Det är avancerat, men du kan göra formulären mycket dynamiska på det här sättet.
