---
unique-page-id: 1147001
description: Använda logik för standardregel för smart lista - Marketo Docs - Produktdokumentation
title: Använda logik för standardregel för smart lista
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Använda logik för standardregel för smart lista {#using-standard-smart-list-rule-logic}

Du kanske har märkt alternativet &quot;Använd filter&quot; när du skapar smarta kampanjlistor. Med den här inställningen kan du bestämma om filtren behöver utvärderas med operatorn AND eller OR.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>Om du ändrar logiken för regel för smart lista gäller detta endast filter, **inte** utlösare.

Utlösare utvärderas alltid som ELLER även om inställningen ovan är inställd på ALL.  Här är ett exempel:

![](assets/image2014-9-22-14-3a12-3a57.png)

Ovanstående lista med ord:
`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` Så om en person fyller i formuläret **eller** besöker sidan, kommer kampanjen att utvärdera personen baserat på **all **eller **any **i de efterföljande filtren, beroende på vilken inställning som används.

>[!MORELIKETHIS]
>
>* [Använda avancerad logik för smarta listregler](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



