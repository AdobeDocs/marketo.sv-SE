---
unique-page-id: 2360297
description: Begränsa Marketo-inloggningar baserat på IP - Marketo Docs - produktdokumentation
title: Begränsa Marketo-inloggningar baserat på IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 3595cdc76a0f92da10dc5ddaac64c4cf83056e88
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Begränsa Marketo-inloggningar baserat på IP {#restrict-marketo-logins-based-on-ip}

Du kan begränsa eller göra det möjligt för användare att få åtkomst till Marketo baserat på deras IP-adresser. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!IMPORTANT]
>
>Adobe Admin Console (AAC) stöder [IP-baserad åtkomstkontroll](https://helpx.adobe.com/enterprise/using/ip-based-access.html){target="_blank"}. För att övergången ska gå smidigt kommer befintliga Marketo Engage IP-begränsningar att vara aktiva, inklusive Adobe ID-användare till och med Q1 2026 i prenumerationer där den här funktionen är aktiverad.
>
>* Du kan konfigurera AAC IP-baserad åtkomst när som helst.
>* Både AAC- och Marketo Engage-begränsningar kan köras samtidigt. Använd samma IP-tillåtelselista för kompatibilitet.
>
>Efter 1:a kvartalet 2026 upphör begränsningarna för Marketo Engage IP. IP-baserad åtkomst hanteras exklusivt via AAC och måste konfigureras för att framtvinga inloggningsbegränsningar. Ett slutligt övergångsdatum kommer att tillkännages senare.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Klicka på **[!UICONTROL Login Settings]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Klicka på **[!UICONTROL Edit IP Restrictions]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Välj om du vill **Tillåt** eller **Blockera** specifika adresser, ange adressen/adresserna och klicka sedan på **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **[!UICONTROL Allowed IP addresses]**: Tillåtna IP-adresser läggs till. Den kommer att innehålla alla angivna IP-adresser och utesluta allt annat.
   >* **[!UICONTROL Block IP addresses]**: Förhindrar att specifika IP-adresser får åtkomst till Marketo.
   >* **[!UICONTROL Disable IP Restrictions]**: Om du kontrollerar detta kommer alla begränsningsregler att sluta fungera. Använd detta för testning.

   >[!NOTE]
   >
   >Du kan lägga till flera begränsningar, men de kan bara vara ALLA eller ALLA blockerade. Du kan inte blanda och matcha tillåtet och blockerat.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)
