---
unique-page-id: 2360297
description: Begränsa Marketo-inloggningar baserat på IP - Marketo Docs - produktdokumentation
title: Begränsa Marketo-inloggningar baserat på IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Begränsa Marketo-inloggningar baserat på IP {#restrict-marketo-logins-based-on-ip}

Du kan begränsa eller göra det möjligt för användare att få åtkomst till Marketo baserat på deras IP-adresser. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Informationen i den här artikeln gäller endast för direkta inloggningar på login.marketo.com. Det är för närvarande inte möjligt att tillämpa IP-begränsningar för enkel inloggning (SSO).

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Klicka på **[!UICONTROL Login Settings]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Klicka på **[!UICONTROL Edit IP Restrictions]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Välj om du vill **Tillåt** eller **Blockera** anger du adressen/adresserna och klickar sedan på **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **[!UICONTROL Allowed IP addresses]**: Tillåtna IP-adresser läggs till. Den kommer att innehålla alla angivna IP-adresser och utesluta allt annat.
   >* **[!UICONTROL Block IP addresses]**: Förhindrar att specifika IP-adresser får åtkomst till Marketo.
   >* **[!UICONTROL Disable IP Restrictions]**: Om du kontrollerar detta kommer eventuella begränsningsregler att sluta fungera. Använd detta för testning.

   >[!NOTE]
   >
   >Du kan lägga till flera begränsningar, men de kan bara vara ALLA eller ALLA blockerade. Du kan inte blanda och matcha tillåtet och blockerat.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Tack och lov är era marknadsföringsdata nu säkrare än någonsin!
