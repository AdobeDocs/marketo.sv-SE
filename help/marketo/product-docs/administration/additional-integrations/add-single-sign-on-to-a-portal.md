---
unique-page-id: 2360356
description: Lägg till enkel inloggning på en portal - Marketo Docs - produktdokumentation
title: Lägg till enkel inloggning på en portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Lägg till enkel inloggning på en portal {#add-single-sign-on-to-a-portal}

Om du har en katalogtjänst som autentiserar användare kan du tillåta enkel inloggning (SSO) i Marketo. Vi stöder den här funktionen med SAML (Security Assertion Markup Language) version 2.0 och senare.

Marketo fungerar som en SAML-tjänsteleverantör (SP) och är beroende av en extern identitetsleverantör (IdP) för att autentisera användare.

När enkel inloggning är aktiverad kan IdP validera användarens inloggningsuppgifter. När en användare vill använda Marketo-programvara skickar IdP sedan ett signerat SAML-meddelande till Marketo, som fungerar som SP. Det här meddelandet garanterar Marketo att användaren har behörighet att använda Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Är du en Microsoft Azure-användare? Kolla in deras [självstudiekurs om integrering](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target=&quot;_blank&quot;}.

## Skicka förfrågan {#how-to-send-the-request}

* Skicka SSO-begäran, som är ett SAML-svar, till `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Som SP:s målgrupps-URL. Använd `http://saml.marketo.com/sp`
* Om du använder attributet SPNameQualifier anger du att elementet NameID för Subject ska vara `http://saml.marketo.com/sp`
* Om du federerar flera Marketo-prenumerationer till samma SSO-leverantör kan du använda unika SP-URL:er för varje Marketo-underordnad med formatet `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo stöder endast Identity Provider-initierad (kallas även IdP-initierad), där användaren först startar Idp-inloggningssidan, autentiserar och sedan navigerar till Min Marketo.

## Ytterligare information {#additional-notes}

* **Synkroniseringstid** - För en ny användare sker en fördröjning på cirka 10 minuter innan en första enkel inloggningsbegäran behandlas.
* **Användaretablering** - Användare etableras manuellt av Marketo.
* **Behörighet** - Användarbehörigheter behålls inom Marketo.
* **Stöd för OAuth** - Marketo stöder för närvarande inte OAuth.
* **Automatisk användarspridning** - Kallas även&quot;Just in Time Provisioning&quot;, det här är när en användares första SAML-inloggning kan skapa användaren i något webbprogram som han/hon använder (t.ex. Marketo) och ingen manuell administratörsåtgärd krävs. Detta stöds för närvarande inte av Marketo.
* **Kryptering** - Marketo stöder för närvarande inte kryptering.

>[!NOTE]
>
>Innan du startar bör du ha ditt identitetsleverantörscertifikat i X.509-format och i filnamnstillägget .crt, .der eller .cer.

## Uppdatera SAML-inställningar {#update-saml-settings}

SSO är inaktiverat som standard. Följ de här stegen för att aktivera SAML och konfigurera det.

1. Gå till **Administratör** område.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Klicka **Enkel inloggning**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Om du inte ser **Enkel inloggning** under **Administratör**, kontakt [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}.

1. Under **SAML-inställningar** avsnitt, klicka **Redigera**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Ändra **SAML enkel inloggning** till **Aktiverad**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Ange **Utfärdar-ID**, **Enhets-ID** väljer du **Plats för användar-ID** och sedan klicka **Bläddra**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Välj **Certifikat för identitetsleverantör** -fil.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Klicka **Spara**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Uppdatera inställningar för omdirigeringssida {#update-redirect-page-settings}

1. Under **Omdirigera sidor** avsnitt, klicka **Redigera**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Kunder som använder Universal ID tillsammans med enkel inloggning måste ange identitetsleverantörens inloggnings-URL i **Inloggnings-URL** fält.

1. Ange **Utloggnings-URL**. Det här är den URL som du vill att användaren ska dirigeras till när han/hon loggar ut från Marketo.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Ange en **Fel-URL**. Det här är den URL som du vill att användaren ska dirigeras till om inloggningen till Marketo misslyckas. Klicka **Spara**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Båda dessa sidor måste vara allmänt tillgängliga.

>[!MORELIKETHIS]
>
>* [Använda ett universellt ID för prenumerationsinloggning](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target=&quot;_blank&quot;}
>* [Begränsa användarinloggning till enbart enkel inloggning](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target=&quot;_blank&quot;}
>* [Bjud in Marketo-användare till två instanser med Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target=&quot;_blank&quot;}

