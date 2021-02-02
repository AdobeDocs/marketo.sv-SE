---
unique-page-id: 12983390
description: Registrera en app med Azure för att hämta ditt klient-ID/program-ID - Marketo Docs - Produktdokumentation
title: Registrera en app med Azure för att hämta ditt klient-ID/program-ID
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Registrera en app med Azure för att hämta ditt klient-ID/program-ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory utökar dina lokala kataloger till molnet, vilket ger stöd för MS Dynamics 365 CRM med lokal ADFS-autentisering.

## Registrerar en ny app {#registering-a-new-app}

1. [Logga ](http://manage.windowsazure.com/) in på Microsoft Azure-hanteringsportalen med ett konto med administratörsbehörighet. Du kan även komma åt Microsoft Azure-portalen via administrationscentret för Office 365 genom att expandera **Admin**-objektet i den vänstra navigeringsrutan och välja **Azure AD**.

   >[!CAUTION]
   >
   >Du måste använda ett konto i samma Office 365-prenumeration som du tänker registrera appen med.

   >[!NOTE]
   >
   >Om du inte har något Azure-konto kan du [registrera dig](https://azure.microsoft.com/en-us/free/) för ett. Läs Microsoft-dokumentationen eller kontakta din Microsoft-representant om du vill ha mer information. När du har skapat ett Azure-konto kan du registrera ett eller flera program med hjälp av proceduren som beskrivs nedan.
   >
   >
   >Om du har ett Azure-konto men din Office 365-prenumeration med Microsoft Dynamics 365 inte är tillgänglig i din Azure-prenumeration följer du [dessa instruktioner](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) för att associera de två kontona.

1. Sök och klicka på **Azure Active Directory** i den vänstra navigeringsrutan.

   ![](assets/two.png)

1. Klicka på **Programregistreringar** under Hantera.

   ![](assets/three.png)

1. Klicka på **Ny registrering** överst på sidan.

   ![](assets/four.png)

1. Ange ett namn för din app, välj kontotyp och ange en omdirigerings-URL. Klicka sedan på **Registrera** längst ned på sidan.

   ![](assets/five.png)

1. Du bör nu se din app på fliken **Programregistreringar**.

   ![](assets/six.png)

## Konfigurerar programbehörigheter {#configuring-app-permissions}

1. Klicka på det program du vill konfigurera behörigheter för under fliken **Programregistreringar** i din Active Directory.

   ![](assets/seven.png)

1. Klicka på **API-behörigheter** under Hantera.

   ![](assets/eight.png)

1. Klicka på knappen **Lägg till en behörighet**.

   ![](assets/nine.png)

1. Välj **Dynamics CRM**.

   ![](assets/ten.png)

1. Markera rutan **Använd gemensam datatjänst som organisationsanvändare***s** och klicka sedan på **Lägg till behörigheter.**

   ![](assets/eleven.png)

1. När behörigheterna har lagts till, vänta minst 10 sekunder.

   ![](assets/twelve.png)

1. Klicka på **Bevilja administratörens samtycke**.

   ![](assets/thirteen.png)

1. Bekräfta genom att klicka på **Ja**.

   ![](assets/fourteen.png)

   Och du är klar!

   ![](assets/fifteen.png)

