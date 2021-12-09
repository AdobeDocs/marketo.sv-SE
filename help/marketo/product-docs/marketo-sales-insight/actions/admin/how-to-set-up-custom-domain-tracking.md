---
description: Konfigurera anpassad domänspårning - Marketo Docs - produktdokumentation
title: Konfigurera anpassad domänspårning
hide: true
hidefromtoc: true
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Konfigurera anpassad domänspårning {#how-to-set-up-custom-domain-tracking}

Med anpassad domänspårning kan ditt team använda ditt eget företagsnamn i alla spårbara länkar som läggs till i dina säljmeddelanden. När du har konfigurerat det här tillåtslista vi alla länkar du har i ditt e-postmeddelande så att de visas som go.yourcompany.com, så att när någon hovrar över en länk läses de som go.yourcompany.com i stället för go.toutapp.com.

Du behöver hjälp av IT-teamet för att konfigurera en CNAME-post för din domän som pekar på go.toutapp.com. Den här CNAME-filen visas på alla spårningslänkar (t.ex. go.yourcompany.com).

När du har bekräftat för IT-teamet att CNAME är korrekt konfigurerat kan du lägga till det på sidan Anpassad domänspårning i Åtgärder.

>[!NOTE]
>
>Om CNAME inte är korrekt konfigurerat och du aktiverar det som din anpassade domän i Åtgärder kan det bryta spårningslänkar och pixlar.

## Aktivera anpassad domänspårning {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Administratörsprivilegier krävs.**

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. Under Administratörsinställningar väljer du **Spårning**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Ange ditt CNAME-namn på fliken Anpassad domänspårning och klicka på **Anslut**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
