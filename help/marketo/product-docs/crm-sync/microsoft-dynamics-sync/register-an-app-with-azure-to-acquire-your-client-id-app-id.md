---
unique-page-id: 12983390
description: Registrera en app med Azure för att hämta ditt klient-ID/program-ID - Marketo Docs - produktdokumentation
title: Registrera en app med Azure för att hämta ditt klient-ID/program-ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Registrera en app med Azure för att hämta ditt klient-ID/program-ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory utökar dina lokala kataloger till molnet, vilket ger stöd för MS Dynamics 365 CRM med lokal ADFS-autentisering.

## Registrera en ny app {#registering-a-new-app}

1. [Logga in](https://login.microsoftonline.com/){target=&quot;_blank&quot;} till Microsoft Azure-hanteringsportalen med ett konto med administratörsbehörighet. Du kan även komma åt Microsoft Azure-portalen via administrationscentret för Office 365 genom att utöka **Administratör** objekt i den vänstra navigeringsrutan och markera **Azure AD**.

   >[!CAUTION]
   >
   >Du måste använda ett konto i samma Office 365-prenumeration som du tänker registrera appen med.

   >[!NOTE]
   >
   >Om du inte har något Azure-konto kan du [registrera dig](https://azure.microsoft.com/en-us/free/){target=&quot;_blank&quot;} för en. Läs Microsoft dokumentation eller kontakta Microsoft för mer information. När du har skapat ett Azure-konto kan du registrera ett eller flera program med hjälp av proceduren som beskrivs nedan.
   >
   >
   >Om du har ett Azure-konto men din Office 365-prenumeration med Microsoft Dynamics 365 inte är tillgänglig i din Azure-prenumeration följer du [dessa instruktioner](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target=&quot;_blank&quot;} för att associera de två kontona.

1. Sök och klicka **Azure Active Directory** i den vänstra navigeringsrutan.

   ![](assets/two.png)

1. Under Hantera klickar du på **Appregistreringar**.

   ![](assets/three.png)

1. Klicka **Ny registrering** överst på sidan.

   ![](assets/four.png)

1. Ange ett namn för din app, välj kontotyp och ange en omdirigerings-URL. Klicka sedan på **Registrera** längst ned på sidan.

   ![](assets/five.png)

1. Du bör nu se din app i **Appregistreringar** -fliken.

   ![](assets/six.png)

## Konfigurera programbehörigheter {#configuring-app-permissions}

1. Under **Appregistreringar** i din Active Directory klickar du på det program du vill konfigurera behörigheter för.

   ![](assets/seven.png)

1. Under Hantera klickar du på **API-behörigheter**.

   ![](assets/eight.png)

1. Klicka på **Lägg till en behörighet** -knappen.

   ![](assets/nine.png)

1. Välj **Dynamics CRM**.

   ![](assets/ten.png)

1. Kontrollera **Få tillgång till gemensam datatjänst som organisationsanvändare***s** och klicka sedan på **Lägg till behörigheter.**

   ![](assets/eleven.png)

1. När behörigheterna har lagts till, vänta minst 10 sekunder.

   ![](assets/twelve.png)

1. Klicka på **Medgivande från bidragsadministratör** -knappen.

   ![](assets/thirteen.png)

1. Klicka **Ja** för att bekräfta.

   ![](assets/fourteen.png)

   Och du är klar!

   ![](assets/fifteen.png)
