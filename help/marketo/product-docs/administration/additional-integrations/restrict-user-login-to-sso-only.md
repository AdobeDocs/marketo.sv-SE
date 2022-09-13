---
unique-page-id: 2360358
description: Begränsa användarinloggning till enbart enkel inloggning - Marketo Docs - produktdokumentation
title: Begränsa användarinloggning till enbart enkel inloggning
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: 5dcaf886c488e5e1b7fd1c4caa5f869e70c6fb18
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Begränsa användarinloggning till enbart enkel inloggning {#restrict-user-login-to-sso-only}

Om du är [med SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) och vill vara säker på att användarna inte kan kringgå SSO-säkerheten ska du följa dessa instruktioner.

>[!IMPORTANT]
>
>Den här artikeln gäller inte för [Adobe IMS-aktiverad](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo prenumerationer.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Administratör** och klicka **Inloggningsinställningar**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Klicka **Redigera skyddsinställningar**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Expandera de avancerade inställningarna, kontrollera **Kräv enkel inloggning** och klicka **Spara**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Det bästa sättet är att bjuda in och acceptera inbjudan. _Efter_ När inbjudan har accepterats bör administratörer ange dem som&quot;Kräv enkel inloggning&quot;.

>[!TIP]
>
>Om du väljer **Kräv enkel inloggning** kan du utesluta [användarroll](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) från denna begränsning genom att kontrollera **Hoppa över enkel inloggning** när rollen konfigureras. Detta gör att användarna kan logga in normalt. Administratörsanvändare kan till exempel fortfarande behöva logga in på Marketo via inloggningsskärmen.

>[!CAUTION]
>
>När nya användare bjuds in får de e-postinbjudningar. Om **Kräv enkel inloggning** är markerat får de inte dessa e-postmeddelanden, såvida de inte har tilldelats en roll som är inställd på **Hoppa över enkel inloggning**.

Så ja! Nu kommer alla användare (utom användare med behörighet att kringgå enkel inloggning) att begränsas till att endast använda enkel inloggning.

>[!MORELIKETHIS]
>
>* [Lägg till enkel inloggning på en portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Använda ett universellt ID för prenumerationsinloggning](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Bjud in Marketo-användare till två instanser med Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

