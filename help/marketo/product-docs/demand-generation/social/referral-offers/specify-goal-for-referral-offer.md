---
unique-page-id: 2359791
description: Ange mål för hänvisningserbjudande - Marketo Docs - produktdokumentation
title: Ange mål för hänvisningserbjudande
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Ange mål för hänvisningserbjudande {#specify-goal-for-referral-offer}

När du [skapar ett hänvisningserbjudande](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) måste du definiera uppfyllandemålet. Målet kan definieras av personaktivitet på webbsidan, till exempel sidbesök eller registreringar. Du kan till och med använda en [anpassad JavaScript-händelse](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Du kan också använda en smart listutlösare i Marketo för att vänta på en milstolpe, till exempel att en möjlighet skapas för den refererade personen.

Exempelmål:

* 10 hänskjutna besök
* 5 refererade registreringar
* 1 refererad affärsmöjlighet skapad
* 2 refererade e-handelsköp
* 5 refererade webbinarium-deltagare

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Markera hänvisningserbjudandet och klicka på **Redigera utkast**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Gå till **Appinställningar** > **Erbjudandeinformation** i redigeraren för hänvisningserbjudanden.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Under **Inställningar** väljer du en händelsetyp i listrutan **Uppfyllandemål**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Om du tänker använda flödessteget **Ge kredit till referent** måste du välja **Smart List-utlösare** som måltyp för uppfyllelse här.

* Refererade besök: Erbjud deltagare beröm för varje besök från en vän till den sida som är värd för ditt erbjudande.
* Refererade signeringsavtal: Erbjudandedeltagare får kredit för varje vän som registrerar sig för erbjudandet.
* Smart List-utlösare: Erbjudandedeltagare får kredit för varje vän som uppfyller villkoren för en [smart listutlösare](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) i en [smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Du kan till exempel använda en utlösare som aktiveras när en refererad potentiell kund registrerar sig för ett webbinarium.

* Anpassad JavaScript-händelse: Erbjudandedeltagare får beröm för varje vän som utlöser en definierad JavaScript-händelse på din sida. Se [Konverteringsskript för anpassade händelser](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Det finns nya filter och utlösare tillgängliga i smarta kampanjer för att övervaka den sociala aktiviteten. Se [använd utlösare och filter för sociala aktiviteter](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Sedan kan du [välja e-postmeddelanden om registrering och uppfyllelse](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) som du vill skicka från ditt hänvisningserbjudande.
