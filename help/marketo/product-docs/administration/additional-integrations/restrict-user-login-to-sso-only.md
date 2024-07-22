---
unique-page-id: 2360358
description: Begränsa användarinloggning till enbart enkel inloggning - Marketo Docs - produktdokumentation
title: Begränsa användarinloggning till enbart enkel inloggning
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Begränsa användarinloggning till enbart enkel inloggning {#restrict-user-login-to-sso-only}

Om du [använder enkel inloggning](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) och vill vara säker på att användarna inte kan kringgå enkel inloggning följer du dessa instruktioner.

>[!IMPORTANT]
>
>Den här artikeln gäller inte för [Adobe IMS-aktiverade](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo-prenumerationer.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Klicka på **[!UICONTROL Login Setting]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Klicka på **[!UICONTROL Edit Security Settings]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Utöka inställningarna för **[!UICONTROL Advanced]**, kontrollera **[!UICONTROL Require SSO]** och klicka på **[!UICONTROL Save]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Det bästa sättet är att bjuda in och acceptera inbjudan. _När inbjudan har accepterats bör administratörer ange dem till [!UICONTROL Require SSO]._

>[!TIP]
>
>Om du väljer **[!UICONTROL Require SSO]** kan du utesluta en [användarroll](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) från den här begränsningen genom att markera alternativet **[!UICONTROL Bypass Single Sign-On]** när du konfigurerar rollen. Detta gör att användarna kan logga in normalt. Administratörsanvändare kan till exempel fortfarande behöva logga in på Marketo via inloggningsskärmen.

>[!CAUTION]
>
>När nya användare bjuds in får de e-postinbjudningar. Om **[!UICONTROL Require SSO]** väljs kommer de inte att få dessa e-postmeddelanden, såvida de inte tilldelats en roll som är inställd på **[!UICONTROL Bypass Single Sign-On]**.

Så ja! Nu kommer alla användare (utom användare med behörighet att kringgå enkel inloggning) att begränsas till att endast använda enkel inloggning.

>[!MORELIKETHIS]
>
>* [Lägg till enkel inloggning i en portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Använder ett universellt ID för prenumerationsinloggning](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Bjuder in Marketo-användare till två instanser med Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
