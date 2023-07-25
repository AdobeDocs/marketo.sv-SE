---
unique-page-id: 1147001
description: Använda logik för standardregel för smart lista - Marketo Docs - produktdokumentation
title: Använda logik för standardregel för smart lista
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Använda logik för standardregel för smart lista {#using-standard-smart-list-rule-logic}

Du kanske har märkt alternativet &quot;Använd filter&quot; när du skapar smarta kampanjlistor. Med den här inställningen kan du bestämma om filtren behöver utvärderas med operatorn AND eller OR.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>Ändringen av regellogik för smarta listor gäller endast filter. **not** -utlösare.

Utlösare utvärderas alltid som ELLER även om inställningen ovan är inställd på ALL.  Här är ett exempel:

![](assets/image2014-9-22-14-3a12-3a57.png)

Ovanstående lista med ord:

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

Så om en person fyller i formuläret **eller** besöker sidan, kommer kampanjen sedan att utvärdera personen baserat på **alla** eller **alla** av de efterföljande filtren, beroende på vilken inställning som används.

>[!MORELIKETHIS]
>
>[Använda avancerad logik för smarta listregler](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
