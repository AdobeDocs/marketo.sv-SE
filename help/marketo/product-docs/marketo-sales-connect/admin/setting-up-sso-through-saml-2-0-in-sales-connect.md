---
unique-page-id: 14352405
description: Lär dig hur du konfigurerar enkel inloggning via SAML 2.0 i Sales Connect. Få krav och konfigurationssteg för din SSO-leverantör och unika domän.
title: Konfigurera enkel inloggning via SAML 2.0 i [!DNL Sales Connect]
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Konfigurera enkel inloggning via SAML 2.0 i [!DNL Sales Connect] {#setting-up-sso-through-saml-in-sales-connect}

Vi stöder enkel inloggning via SAML 2.0-specifikationen. Men vi har för närvarande ingen direkt integrering med någon leverantör. Vi måste samla in viss information från din SSO-leverantör för att få tillgång till den här konfigurationen.

>[!NOTE]
>
>Detta gäller endast för **Marketo Sales Connect**-användare. Om du inte har Sales Connect men vill veta mer kontaktar du Adobe Account Team (din Account Manager).

## Krav {#requirements}

* SSO-konto
* Marketo Sales Connect-prenumeration
* Metadata.xml från SSO-konto (Issue URL, endpoint for validation och a public key)

## Inställningar {#setup}

Metadata.xml från teamets SSO-instans ska innehålla utfärdarens URL, valideringens slutpunkt och en offentlig nyckel.

Vi behöver också SSO-platsen för ditt företags SSO-konto som en unik domän. Vi behöver till exempel en unik underdomän som `toutapp.pingidentity.com` eller liknande. Utan den här typen av unik identifierare kan vi inte konfigurera SAML från kontrollpanelen.

One Login och Okta tillhandahåller inte alltid unika identifierare när en URL tilldelas. Om du använder Okta eller One Login betyder det att vi inte kan konfigurera en inloggning från kontrollpanelsknappen. Vi kommer fortfarande att kunna konfigurera det med knappen för enkel inloggning i [webbprogrammet](https://toutapp.com/login).

När vi har fått den informationen kommer vi att arbeta tillsammans med vårt tekniker för att göra detta för din prenumeration.
