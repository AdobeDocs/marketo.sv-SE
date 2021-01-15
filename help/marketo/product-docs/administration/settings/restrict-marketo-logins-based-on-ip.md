---
unique-page-id: 2360297
description: Begränsa Marketo-inloggningar baserat på IP - Marketo Docs - produktdokumentation
title: Begränsa Marketo-inloggningar baserat på IP
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Begränsa Marketo-inloggningar baserat på IP {#restrict-marketo-logins-based-on-ip}

Du kan begränsa eller göra det möjligt för användare att komma åt Marketo baserat på deras IP-adresser. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Informationen i den här artikeln gäller endast för direkta inloggningar på login.marketo.com. Det är för närvarande inte möjligt att tillämpa IP-begränsningar för enkel inloggning (SSO).

1. Under **Admin** klickar du på **Inloggningsinställningar**.

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. Klicka på **Redigera IP-begränsningar**.

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. Välj om du vill **Tillåt** eller **Blockera** specifika adresser, ange adressen/adresserna och klicka sedan på **Spara**.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **Tillåtna IP-adresser**: Tillåtna IP-adresser läggs till. Den kommer att innehålla alla angivna IP-adresser och utesluta allt annat.
   >* **Blockera IP-adresser**: Förhindrar att specifika IP-adresser kommer åt Marketo.
   >* **Inaktivera IP-begränsningar**: Om du kontrollerar detta kommer eventuella begränsningsregler att sluta fungera. Använd detta för testning.


   >[!NOTE]
   >
   >Du kan lägga till flera begränsningar, men de kan bara vara ALLA eller ALLA blockerade. Du kan inte blanda och matcha tillåtet och blockerat.

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   Tack och lov är era marknadsföringsdata nu säkrare än någonsin!
