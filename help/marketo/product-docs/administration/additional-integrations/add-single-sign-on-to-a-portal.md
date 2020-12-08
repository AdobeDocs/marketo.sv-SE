---
unique-page-id: 2360356
description: Lägg till enkel inloggning i en portal - Marketo Docs - Produktdokumentation
title: Lägg till enkel inloggning på en portal
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# Lägg till enkel inloggning på en portal {#add-single-sign-on-to-a-portal}

Om du har en katalogtjänst som autentiserar användare kan du tillåta enkel inloggning (SSO) i Marketo. Vi stöder den här funktionen med SAML (Security Assertion Markup Language) version 2.0 och senare.

Marketo fungerar som en SAML Service Provider (SP) och är beroende av en extern identitetsleverantör (IdP) för att autentisera användare.

När enkel inloggning är aktiverad kan IdP validera användarens inloggningsuppgifter. När en användare vill använda Marketo skickar IdP sedan ett signerat SAML-meddelande till Marketo, som fungerar som SP. Det här meddelandet bekräftar för Marketo att användaren har behörighet att använda Marketo.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Är du en Microsoft Azure-användare? Kolla in deras [integreringsjälvstudiekurs](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Skicka förfrågan {#how-to-send-the-request}

* Skicka SSO-begäran, som är ett SAML-svar, till `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Som SP:s målgrupps-URL. Använd [http://saml.marketo.com/sp](http://saml.marketo.com/sp)
* Om du använder attributet SPNameQualifier anger du [http://saml.marketo.com/sp för elementet NameID för Subject](http://saml.marketo.com/sp)
* Om du federerar flera Marketo-prenumerationer till samma SSO-leverantör kan du använda unika SP-URL:er för varje Marketo-underordnad med formatet `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo stöder endast Identity Provider-initierad (kallas även IdP-initierad) där användaren först startar Idp-inloggningssidan, autentiserar och sedan navigerar till My Marketo.

## Ytterligare information {#additional-notes}

* **Synkroniseringstid** - För en ny användare uppstår cirka 10 minuters fördröjning innan en första enkel inloggningsbegäran behandlas.
* **Användaretablering** - Användare etableras manuellt av Marketo.
* **Autentisering** - Användarbehörigheter behålls i Marketo.
* **OAuth-stöd** - Marketo stöder för närvarande inte OAuth.

>[!NOTE]
>
>Innan du startar bör du ha ditt identitetsleverantörscertifikat i X.509-format och i filnamnstillägget .crt, .der eller .cer.

## Uppdatera SAML-inställningar {#update-saml-settings}

SSO är inaktiverat som standard. Följ de här stegen för att aktivera SAML och konfigurera det.

1. Gå till **Admin **och klicka på **enkel inloggning**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Om du inte ser **enkel inloggning** under **Admin** kontaktar du [`[email protected]`](http://mailto:support@marketo.com).

1. Klicka på **Redigera** under avsnittet **SAML-inställningar**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Ändra **SAML enkel inloggning** till **aktiverad**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Ange **utfärdarens ID**, **enhets-ID**, markera platsen **för** användar-ID och klicka sedan på **Bläddra**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Välj **identitetsleverantörens certifikatfil** .

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Klicka på **Spara**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Uppdatera inställningar för omdirigeringssida {#update-redirect-page-settings}

1. Klicka på **Redigera** under avsnittet **Omdirigera sidor**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Kunder som använder Universal ID tillsammans med enkel inloggning måste ange identitetsleverantörens inloggnings-URL i fältet **Inloggnings-URL** .

1. Ange en **utloggnings-URL**. Det här är den URL som du vill att användaren ska dirigeras till när han/hon loggar ut från Marketo.

   ![](assets/eight.png)

1. Ange en **fel-URL**. Det här är den URL som du vill att användaren ska dirigeras till om det inte går att logga in på Marketo. Klicka på **Spara**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Båda dessa sidor måste vara allmänt tillgängliga.

