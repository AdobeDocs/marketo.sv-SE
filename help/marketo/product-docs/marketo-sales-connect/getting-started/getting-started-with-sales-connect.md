---
unique-page-id: 13796466
description: Komma igång med Sales Connect - Marketo Docs - produktdokumentation
title: Komma igång med Sales Connect
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Komma igång med Sales Connect {#getting-started-with-sales-connect}

Om du hellre vill titta på de här stegen än att läsa dem går du direkt till [videoinstruktionerna nedan](#video).

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din Customer Success Manager om du vill ha mer information.

## Vad du behöver för att komma igång {#what-you-need-to-get-started}

* Marketo-prenumeration
* prenumeration på Sales Connect
* Salesforce-prenumeration (med API-anrop och Apex-klasser aktiverade)

## Vem du behöver för att komma igång {#who-you-need-to-get-started}

* Marketo Admin-användare
* Administratörsanvändare för Sales Connect
* Salesforce-administratör
* Sales Connect-användare

## Administratörer för Sales Connect {#sales-connect-admins}

Du får ett e-postmeddelande från Marketo med en länk för att återställa ditt lösenord. När du har skapat ett nytt lösenord loggar du in på Sales Connect.

För att slutföra installationen måste du göra följande:

* [Connect Sales Connect och Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [Hämta autentiseringsuppgifter innan du ansluter säljaren till Marketo](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Connect Sales Connect with Marketo](#connect-sales-connect-to-marketo)
* [Bjud in/etablera användare](#invite-provision-users)

Du kan också:

* [Testa Sales Connect i din sandlåda](#test-sales-connect-in-your-sandbox)

## Anslut ditt Sales Connect-konto till Salesforce {#connect-your-sales-connect-account-to-salesforce}

Om du vill ansluta ditt Sales Connect-konto till ditt Salesforce-konto, som administratör eller annan administratör, följer du stegen i [den här artikeln](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md).

>[!NOTE]
>
>Den instans av Salesforce som du ansluter till måste vara samma instans som är (eller kommer att vara) ansluten till Marketo.

## Hämtar autentiseringsuppgifter innan du ansluter försäljningen Anslut till Marketo {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Du måste hämta en uppsättning inloggningsuppgifter inifrån Marketo. Dessa autentiseringsuppgifter används senare av Sales Connect Admin för att ansluta Marketo till Sales Connect.

1. Klicka på **Admin** i Marketo.

   ![](assets/one.png)

1. Klicka på **Sales Connect** i trädet.

   ![](assets/two.png)

1. Välj och skicka följande Marketo-autentiseringsuppgifter till din Sales Connect-administratör: Munchkin-ID, klient-ID, klienthemlighet.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >När du kopierar och klistrar in ovanstående information bör du kontrollera att inga mellanslag läggs till.

## Anslut försäljningsanslutning till Marketo {#connect-sales-connect-to-marketo}

1. Klicka på kugghjulsikonen i Sales Connect och välj **Inställningar**.

   ![](assets/four.png)

1. Under Administratörsinställningar väljer du **Marketo**.

   ![](assets/eight.png)

1. Ange de Marketo-autentiseringsuppgifter som tillhandahålls av Marketo Admin och klicka på **Anslut**.

   ![](assets/credentials.png)

## Bjud in/etablera användare {#invite-provision-users}

Om det redan finns användare på ditt konto (tidigare från ToutApp) visas de på fliken **Teamåtkomst** i Marketo-delen av Sales Connect.

Du kan distribuera ditt team som Marketo Sales Connect User från den här sidan. Om du aldrig har använt ToutApp, eller ännu inte har bjudit in användare, följer du stegen i [den här artikeln](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md).

>[!CAUTION]
>
>Vänta tio minuter efter att du har anslutit Sales Connect till Marketo innan du utför dessa steg.

1. Markera en eller flera användare och klicka sedan på **Anslut**.

   >[!NOTE]
   >
   >Du kan bara utföra arbetsytetilldelningen en gång när du bjuder in användare. När den är inställd måste du koppla från användaren för att kunna ändra den.

   ![](assets/users.png)

1. Om din Marketo-prenumeration har arbetsytor aktiverade kan du tilldela arbetsytor till alla användare eller grupper av användare samtidigt. Om inga arbetsytor är markerade tilldelas de till Marketo standardarbetsyta.

   ![](assets/nine.jpg)

1. Klicka på listrutan Arbetsyta, välj önskad arbetsyta och klicka på **Anslut**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Om du vill lägga till nya användare går du till avsnittet Teamhantering i Administrationsinställningar och klickar på knappen **Bjud in användare**.

Du kan få fler användare från sidan Teamhantering och följa stegen ovan för att få dem anslutna.

## Testa Säljanslutning i din sandlåda {#test-sales-connect-in-your-sandbox}

För team som vill testa Marketo Sales Connect med sin Marketo Sandbox kan ytterligare ett Sales Connect-konto etableras på begäran. Detta gäller endast kunder som har köpt en Marketo Sandbox, eller kunder som har den som en del av deras Marketo-paket. Kontakta din kontoansvarige på Marketo om du är intresserad av att köpa en sandlåda.

>[!NOTE]
>
>Du kan inte etablera ett Sales Connect-konto med samma e-post-ID till flera instanser. Det innebär att om du vill ha ett extra Sales Connect-konto för att testa med din Marketo Sandbox-instans måste du använda ett annat e-post-ID för varje konto.
