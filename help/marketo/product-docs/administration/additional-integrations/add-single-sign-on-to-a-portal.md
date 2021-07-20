---
unique-page-id: 2360356
description: Lägg till enkel inloggning på en portal - Marketo Docs - produktdokumentation
title: Lägg till enkel inloggning på en portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '0'
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
>Är du en Microsoft Azure-användare? Ta en titt på deras [självstudiekurs om integrering](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Skicka förfrågan {#how-to-send-the-request}

* Skicka SSO-begäran, som är ett SAML-svar, till `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Som SP:s målgrupps-URL. Använd `http://saml.marketo.com/sp`
* Om du använder SPNameQualifier-attributet anger du `http://saml.marketo.com/sp` för NameID-elementet för Subject
* Om du federerar flera Marketo-prenumerationer till samma SSO-leverantör kan du använda unika SP-URL:er för varje Marketo-underordnad med formatet `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo stöder endast Identity Provider-initierad (kallas även IdP-initierad), där användaren först startar Idp-inloggningssidan, autentiserar och sedan navigerar till Min Marketo.

## Ytterligare information {#additional-notes}

* **Synkroniseringstid**  - För en ny användare sker cirka 10 minuters fördröjning innan en första enkel inloggningsbegäran behandlas.
* **Användaretablering**  - Användare etableras manuellt av Marketo.
* **Behörighet**  - Användarbehörigheter finns i Marketo.
* **Stöd**  för OAuth - Marketo stöder för närvarande inte OAuth.
* **Automatisk användarspridning**  - Kallas även&quot;Just in Time Provisioning&quot;, det här är när en användares första SAML-inloggning kan skapa användaren i något webbprogram som han/hon använder (t.ex. Marketo) och ingen manuell administratörsåtgärd krävs. Detta stöds för närvarande inte av Marketo.
* **Kryptering**  - Marketo stöder för närvarande inte kryptering.

>[!NOTE]
>
>Innan du startar bör du ha ditt identitetsleverantörscertifikat i X.509-format och i filnamnstillägget .crt, .der eller .cer.

## Uppdatera SAML-inställningar {#update-saml-settings}

SSO är inaktiverat som standard. Följ de här stegen för att aktivera SAML och konfigurera det.

1. Gå till **Admin** och klicka på **Enkel inloggning**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Om du inte ser **enkel inloggning** under **Admin**, kontaktar du [Marketo support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Klicka på **Redigera** under **SAML-inställningar**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Ändra **SAML enkel inloggning** till **Aktiverad**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Ange ditt **Issuer ID**, **Entity ID**, välj **User ID Location** och klicka sedan på **Browse**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Välj din **identitetsleverantörscertifikatfil**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Klicka på **Spara**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Uppdatera inställningar för omdirigeringssida {#update-redirect-page-settings}

1. Klicka på **Redigera** under **Omdirigera sidor**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Kunder som använder Universal ID tillsammans med enkel inloggning måste ange identitetsleverantörens inloggnings-URL i fältet **Inloggnings-URL**.

1. Ange en **Logout URL**. Det här är den URL som du vill att användaren ska dirigeras till när han/hon loggar ut från Marketo.

   ![](assets/eight.png)

1. Ange en **fel-URL**. Det här är den URL som du vill att användaren ska dirigeras till om inloggningen till Marketo misslyckas. Klicka på **Spara**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Båda dessa sidor måste vara allmänt tillgängliga.

>[!MORELIKETHIS]
>
>* [Använda ett universellt ID för prenumerationsinloggning](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
* [Begränsa användarinloggning till enbart enkel inloggning](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
* [Bjud in Marketo-användare till två instanser med Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

