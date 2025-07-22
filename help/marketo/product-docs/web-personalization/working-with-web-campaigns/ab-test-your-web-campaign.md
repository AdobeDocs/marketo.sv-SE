---
unique-page-id: 4719404
description: AB Testa din webbkampanj - Marketo Docs - Produktdokumentation
title: AB Testa webbkampanjen
exl-id: 65d61b96-d39b-4388-971d-260c9c0aff93
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# AB Testa webbkampanjen {#ab-test-your-web-campaign}

Testning är ett bra sätt att optimera webbkampanjer för bättre engagemang. Så här kommer du igång.

Om du vill A/B-testa dina anpassade kampanjer kan du välja två eller flera kampanjer, associera dem till samma **[!UICONTROL Split Test]**-grupp och välja **[!UICONTROL Auto Tune]** för att automatiskt fortsätta med den bästa kampanjen.

>[!TIP]
>
>Aktivera inte [!UICONTROL Auto Tune] om du föredrar att manuellt beräkna och se vilken kampanj som fungerar bäst.

## Konfigurera ett delat A/B-test {#how-to-set-up-a-split-a-b-test}

1. Gå till **[!UICONTROL Web Campaigns]**.

   ![](assets/web-campaigns-hand-2.jpg)

   >[!NOTE]
   >
   >Använd [filterfunktionen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md) för att göra det enklare att hitta kampanjen.

1. Välj den första kampanjen som du vill göra ett A/B-test. Klicka på **[!UICONTROL Edit]**.

   ![](assets/image2016-11-4-13-3a46-3a37.png)

1. Välj **[!UICONTROL Split Testing]** på kampanjsidan och klicka på **[!UICONTROL Create New]**.

   ![](assets/image2014-11-26-16-3a47-3a18.png)

1. Ange **namnet på den delade testgruppen** och klicka på **[!UICONTROL Create]**. Välj **[!UICONTROL Auto Tune]**.

   ![](assets/image2014-11-26-16-3a52-3a24.png)

1. **[!UICONTROL Save]** eller **[!UICONTROL Launch]** kampanjen.

   >[!TIP]
   >
   >Om du väljer **[!UICONTROL Auto Tune]** kan plattformen [!DNL Web Personalization] automatiskt känna igen den bättre delade testkampanjen och fortsätta med den högsta konverteringskampanjen samtidigt som de andra pausas.

1. Upprepa ovanstående process med den andra kampanjen.

1. Välj den andra kampanjen som du vill göra A/B-test. Klicka på **[!UICONTROL Edit]**.

   ![](assets/image2016-11-4-13-3a51-3a39.png)

1. Välj **[!UICONTROL Set Campaign]** Dela testning **på sidan** och välj **Grupp** i listrutan. Välj **[!UICONTROL Auto Tune]**.

   ![](assets/image2014-11-26-17-3a2-3a17.png)

1. **[!UICONTROL Save]** eller **[!UICONTROL Launch]** kampanjen.

1. Upprepa den här processen för en tredje eller fjärde kampanj att testa.

1. I **[!UICONTROL Web Campaigns]** kan du se de delade testkampanjerna som A/B-ikonen anger.

   ![](assets/image2016-11-4-13-3a55-3a5.png)

>[!TIP]
>
>1. Ni kan testa så många kampanjer ni vill. Bästa praxis är två till tre kampanjer
>1. Se till att varje delad testgrupp är associerad med samma segment. Ni vill testa mot samma målgrupp.
>1. Testa olika delar av materialet (fallstudie A vs. fallstudie B), ändra budskap och kreatörer, färger, storlekar eller anrop till olika aktiviteter.
>1. Optimera och njut av ert personaliserade innehåll!

>[!MORELIKETHIS]
>
>* [Skapa en dialogkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Skapa en RTP i zonkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Skapa en Widget-kampanj för RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
