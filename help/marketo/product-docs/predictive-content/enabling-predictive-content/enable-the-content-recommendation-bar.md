---
unique-page-id: 4720108
description: Aktivera innehållsrekommendationsfältet - Marketo Docs - produktdokumentation
title: Aktivera innehållsrekommendationsfältet
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---


# Aktivera innehållsrekommendationsfältet {#enable-the-content-recommendation-bar}

Innehållsrekommendationsmotorn använder prediktiva analyser och maskininlärningsalgoritmer för att leverera relevant innehåll till varje webbbesökare. Rekommendationsmotorn förutser vilket innehåll som fungerar bäst per besökare. Innehållet i motorn övervakas och styrs under Recommendations-sidan, vilket hjälper dig att optimera avkastningen på ditt innehåll.

>[!PREREQUISITES]
>
>Innan du aktiverar prediktivt innehåll måste du:
>
>* [Förbered ditt prediktiva innehåll](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [Godkänn en titel för prediktivt innehåll](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Aktivera och anpassa innehållsrekommendationsfältet {#enable-and-customize-the-content-recommendation-bar}

1. Gå till **Innehållsinställningar**.

   ![](assets/settings-dropdown-hand.png)

1. Klicka på **Fält**.

   ![](assets/content-settings-bar-hand.png)

1. Om du vill aktivera rekommendationsfältet för en URL-adress klickar du bara på **På** och sedan på **Spara**.

   ![](assets/bar-enable.png)

1. Om du vill anpassa en URL-adress väljer du färger, format, format, pilar för rekommendationsfältet och sidor som ska inkludera eller exkludera fältet. Anpassa sajtens varumärke. Klicka på **Spara**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Inkludera/exkludera visnings-URL**
   >
   >    * URL för visning ska vara domänens sökväg
   >    * Ta inte med http:// eller https://
   >    * Använd * för jokertecken
   * Använda ett semikolon som avgränsare
   * Exempel: /contact_us*; *action=log*
   * Det här fältet är skiftlägeskänsligt


## Överväganden i rekommendationsfältet {#recommendation-bar-considerations}

* Du behöver minst en innehållsdel för rekommendationsfältet som är inställt på **På** på Recommendations-sidan för att rekommendationsmotorn ska fungera. Om inget innehåll är aktiverat och Bar är inställt på **På**, visas effekten Pil längst ned till höger på webbsidan, men inget rekommenderat innehåll visas.

* Ju mer innehåll som körs i rekommendationsmotorn desto bättre för algoritmen att testa och lära sig vilket innehåll som fungerar bäst. Vi rekommenderar att du börjar med 10 till 20 aktiva innehållskomponenter och fortsätter lägga till nya.
* Innehållsdelen som du aktiverar för rekommendation bör innehålla Javascript-taggen RTP. Detta hjälper algoritmen att spåra och optimera rekommenderat innehåll.

>[!NOTE]
**Relaterade artiklar**
* [Aktivera prediktivt innehåll för multimedia för webben](enable-predictive-content-for-web-rich-media.md)

