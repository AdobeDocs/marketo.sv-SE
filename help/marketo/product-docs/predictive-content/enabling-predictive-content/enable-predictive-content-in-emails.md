---
unique-page-id: 11385020
description: Aktivera prediktivt innehåll i e-postmeddelanden - Marketo Docs - produktdokumentation
title: Aktivera prediktivt innehåll i e-postmeddelanden
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# Aktivera prediktivt innehåll i e-postmeddelanden {#enable-predictive-content-in-emails}

Gör en eller flera bilder i ditt e-postmeddelande prediktiva och skräddarsy upplevelsen för varje mottagare.

>[!NOTE]
>
>Vi rekommenderar att du aktiverar över fem innehållsdelar per kategori och källa (e-post, multimedia, fält) innan du testar och använder Predictive Content. Mer innehåll ger ett bättre prediktivt resultat.

>[!PREREQUISITES]
>
>Innan du aktiverar Predictive Content måste du:
>
>* **Förbered ditt prediktiva innehåll**
>
>   * [Redigera prediktivt innehåll för e-postmeddelanden](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} eller
>   * [Redigera förebyggande innehåll för multimedia](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} eller
>   * [Redigera prediktivt innehåll för rekommendationsfältet](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Godkänn en titel för förebyggande innehåll](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Lägga till prediktivt innehåll med e-postredigeraren 2.0 {#adding-predictive-content-using-the-email-editor}

1. Klicka på **[!UICONTROL Marketing Activities]**.

   ![](assets/one.png)

1. Välj din e-postadress och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/two.png)

1. Klicka på bilden som du vill göra prediktiv. När kugghjulsikonen visas klickar du på den och väljer **[!UICONTROL Enable ContentAI]** (ContentAI är det tidigare namnet för Predictive Content).

   ![](assets/three.png)

1. Om du vill markera en eller flera kategorier klickar du på listrutan **[!UICONTROL Categories]**, markerar dem och klickar på **[!UICONTROL Apply]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Det är valfritt att välja specifika kategorier eller ändra den förutsägbara layouten.

1. Bilden är nu prediktiv. Upprepa steg 3 och 4 för ytterligare bilder (om du vill).

   ![](assets/five.png)

1. Om du vill förhandsgranska din e-post klickar du på **[!UICONTROL Preview]** i det övre högra hörnet.

   ![](assets/six.png)

1. Om du vill visa olika möjliga bilder klickar du på **[!UICONTROL Refresh]**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Bilden markeras inte **_förrän mottagaren öppnar e-postmeddelandet_**. Det du ser i förhandsgranskningen är alltså bara ett exempel och behöver inte vara den bild som mottagaren ser.

1. När du har förhandsgranskat e-postmeddelandet klickar du på listrutan **[!UICONTROL Preview Actions]** och väljer **[!UICONTROL Approve and Close]**. Om du fortfarande behöver redigera klickar du på **[!UICONTROL Edit Draft]** till höger.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >När du skickar ett prov markeras en slumpmässig bild.

När du har godkänt ditt e-postmeddelande kommer det att ha prediktivt innehåll och kan skickas!

>[!CAUTION]
>
>När en mottagare öppnar e-postmeddelandet låses prediktiva bilder. Om innehållet tas bort senare visas en trasig bild där innehållet fanns.

## Lägga till prediktivt innehåll när du inte använder e-postredigeraren 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Om du inte använder en [E-post 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"}-mall kan du lägga till prediktivt innehåll i e-postmeddelandet genom att helt enkelt tagga en bild i mallen som ett redigerbart bildelement i Marketo.

Läs mer om den [Marketo-specifika syntaxen här](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Här är ett exempel på hur koden ska se ut (det här är bara ett exempel, kopiera inte koden nedan exakt).

**Exempel**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
