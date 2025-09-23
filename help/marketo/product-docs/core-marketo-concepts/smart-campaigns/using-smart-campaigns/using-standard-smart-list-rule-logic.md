---
unique-page-id: 1147001
description: Använda logik för standardregel för smart lista - Marketo Docs - produktdokumentation
title: Använda logik för standardregel för smart lista
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Använda logik för standardregel för smart lista {#using-standard-smart-list-rule-logic}

Du kan ha märkt alternativet &quot;Använd filter&quot; när du skapade kampanjer med smarta listor. Med den här inställningen kan du bestämma om filtren behöver utvärderas med operatorn AND eller OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>Om du ändrar logik för regel för smart lista gäller detta bara för filter, _inte_ utlösare.

Utlösare utvärderas alltid som ELLER även om inställningen ovan är inställd på ALL. Här är ett exempel:

![](assets/using-standard-smart-list-rule-logic-2.png)

Ovanstående smarta lista med ord:

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

Om en person fyller i formuläret _eller_ besöker sidan, kommer kampanjen sedan att utvärdera personen baserat på _alla_ eller _alla_ efterföljande filter, beroende på vilken inställning som används.

>[!MORELIKETHIS]
>
>[Använder logik för avancerad smart listregel](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
