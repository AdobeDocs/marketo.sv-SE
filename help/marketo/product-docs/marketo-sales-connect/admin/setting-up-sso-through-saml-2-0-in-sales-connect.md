---
unique-page-id: 14352405
description: Konfigurera enkel inloggning via SAML 2.0 i Sales Connect - Marketo Docs - produktdokumentation
title: Konfigurera enkel inloggning via SAML 2.0 i Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Konfigurera enkel inloggning via SAML 2.0 i Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Vi stöder enkel inloggning via SAML 2.0-specifikationen. Men vi har för närvarande ingen direkt integrering med någon leverantör. Vi måste samla in viss information från din SSO-leverantör för att få tillgång till den här konfigurationen.

>[!NOTE]
>
>**Påminnelse**
>
>Detta gäller endast **Marketo Sales Connect** -kunder. Kontakta din Customer Success Manager om du inte har Sales Connect men vill veta mer.

## Krav {#requirements}

* SSO-konto
* Marketo Sales Connect-prenumeration
* Metadata.xml från SSO-konto (Issue URL, endpoint for validation och a public key)

## Inställningar {#setup}

Metadata.xml från teamets SSO-instans ska innehålla utfärdarens URL, valideringens slutpunkt och en offentlig nyckel.

Vi behöver också SSO-platsen för ditt företags SSO-konto som en unik domän. Vi `require a unique subdomain` gillar till exempel&quot;toutapp.pingidentity.com&quot; eller liknande. Utan den här typen av unik identifierare kan vi inte konfigurera SAML från kontrollpanelen.

One Login och Okta tillhandahåller inte alltid unika identifierare när en URL tilldelas. Om du använder Okta eller One Login betyder det att vi inte kan konfigurera en inloggning från kontrollpanelsknappen. Vi kommer fortfarande att kunna konfigurera det med knappen för enkel inloggning i [webbprogrammet](http://toutapp.com/login).

När vi har fått den informationen kommer vi att arbeta tillsammans med vårt tekniker för att göra detta för din prenumeration.
