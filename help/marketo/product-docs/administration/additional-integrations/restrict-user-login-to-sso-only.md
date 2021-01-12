---
unique-page-id: 2360358
description: Begränsa användarinloggning till enbart SSO - Marketo Docs - Produktdokumentation
title: Begränsa användarinloggning till enbart enkel inloggning
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Begränsa användarinloggning till enbart enkel inloggning {#restrict-user-login-to-sso-only}

Om du [använder SSO](add-single-sign-on-to-a-portal.md) och vill vara säker på att användarna inte kan kringgå SSO-säkerheten följer du dessa instruktioner.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Admin** och klicka på **Inloggningsinställningar**.

![](assets/image2014-9-24-14-3a44-3a40.png)

1. Klicka på **Redigera skyddsinställningar**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Utöka de avancerade inställningarna, markera **Kräv enkel inloggning** och klicka på **Spara**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>Om du väljer **Kräv enkel inloggning** kan du utesluta en [användarroll](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) från den här begränsningen genom att markera alternativet **Åsidosätt enkel inloggning** när du konfigurerar rollen. Detta gör att användarna kan logga in normalt. Administratörsanvändare kan till exempel fortfarande behöva logga in på Marketo via inloggningsskärmen.

>[!CAUTION]
>
>När nya användare bjuds in får de e-postinbjudningar. Om **Kräv enkel inloggning** är markerat får de inte dessa e-postmeddelanden, såvida de inte tilldelats en roll som är inställd på **Kringgå enkel inloggning**.

Så ja! Nu kommer alla användare (utom användare med behörighet att kringgå enkel inloggning) att begränsas till att endast använda enkel inloggning.
