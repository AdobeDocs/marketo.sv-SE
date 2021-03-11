---
unique-page-id: 2360358
description: Begränsa användarinloggning till enbart SSO - Marketo Docs - Produktdokumentation
title: Begränsa användarinloggning till enbart enkel inloggning
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Begränsa användarinloggning till enbart enkel inloggning {#restrict-user-login-to-sso-only}

Om du [använder SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) och vill vara säker på att användarna inte kan kringgå SSO-säkerheten följer du dessa instruktioner.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Admin** och klicka på **Inloggningsinställningar**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Klicka på **Redigera skyddsinställningar**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Utöka de avancerade inställningarna, markera **Kräv enkel inloggning** och klicka på **Spara**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Det bästa sättet är att bjuda in och acceptera inbjudan. _När_ inbjudan har accepterats bör administratörer ange dem till Kräv enkel inloggning.

>[!TIP]
>
>Om du väljer **Kräv enkel inloggning** kan du utesluta en [användarroll](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) från den här begränsningen genom att markera alternativet **Åsidosätt enkel inloggning** när du konfigurerar rollen. Detta gör att användarna kan logga in normalt. Administratörsanvändare kan till exempel fortfarande behöva logga in på Marketo via inloggningsskärmen.

>[!CAUTION]
>
>När nya användare bjuds in får de e-postinbjudningar. Om **Kräv enkel inloggning** är markerat får de inte dessa e-postmeddelanden, såvida de inte tilldelats en roll som är inställd på **Kringgå enkel inloggning**.

Så ja! Nu kommer alla användare (utom användare med behörighet att kringgå enkel inloggning) att begränsas till att endast använda enkel inloggning.

>[!MORELIKETHIS]
>
>* [Lägg till enkel inloggning på en portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Använda ett universellt ID för prenumerationsinloggning](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Bjud in Marketo-användare till två instanser med Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

