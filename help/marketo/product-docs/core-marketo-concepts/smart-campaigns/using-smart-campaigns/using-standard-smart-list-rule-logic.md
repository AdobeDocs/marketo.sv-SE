---
unique-page-id: 1147001
description: Använda logik för standardregel för smart lista - Marketo Docs - produktdokumentation
title: Använda logik för standardregel för smart lista
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Använda logik för standardregel för smart lista {#using-standard-smart-list-rule-logic}

Du kan ha märkt alternativet &quot;Använd filter&quot; när du skapade kampanjer med smarta listor. Med den här inställningen kan du bestämma om filtren behöver utvärderas med operatorn AND eller OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>Ändringen av regellogik för smarta listor gäller bara för filter, _not_ -utlösare.

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

Så om en person fyller i formuläret _eller_ besöker sidan, kommer kampanjen sedan att utvärdera den personen baserat på _alla_ eller _alla_ av de efterföljande filtren, beroende på vilken inställning som används.

>[!MORELIKETHIS]
>
>[Använda avancerad logik för smarta listregler](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
