---
unique-page-id: 12983390
description: Registrera en app med Azure för att hämta ditt klient-ID/program-ID - Marketo Docs - produktdokumentation
title: Registrera en app med Azure för att hämta ditt klient-ID/program-ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Registrera en app med Azure för att hämta ditt klient-ID/program-ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory utökar dina lokala kataloger till molnet, vilket ger stöd för [!DNL MS Dynamics 365] CRM med lokal ADFS-autentisering.

## Registrera en ny app {#registering-a-new-app}

1. [Logga in](https://login.microsoftonline.com/){target="_blank"} på Microsoft Azure-hanteringsportalen med ett konto med administratörsbehörighet. Du kan även komma åt Microsoft Azure-portalen via administrationscentret för Office 365 genom att expandera **[!UICONTROL Admin]**-objektet i den vänstra navigeringsrutan och välja **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >Du måste använda ett konto i samma [!DNL Office 365]-prenumeration som den du vill registrera appen med.

   >[!NOTE]
   >
   >Om du inte har något Azure-konto kan du [registrera dig](https://azure.microsoft.com/en-us/free/){target="_blank"} för ett. Läs Microsoft dokumentation eller kontakta Microsoft för mer information. När du har skapat ett Azure-konto kan du registrera ett eller flera program enligt proceduren nedan.
   >
   >
   >Om du har ett Azure-konto men din [!DNL Office 365]-prenumeration med [!DNL Microsoft Dynamics 365] inte är tillgänglig i din Azure-prenumeration följer du [dessa instruktioner](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} för att associera de två kontona.

1. Sök och klicka på **[!UICONTROL Azure Active Directory]** i den vänstra navigeringsrutan.

   ![](assets/two.png)

1. Klicka på [!UICONTROL Manage] under **[!UICONTROL App registrations]**.

   ![](assets/three.png)

1. Klicka på **[!UICONTROL New registration]** överst på sidan.

   ![](assets/four.png)

1. Ange ett namn för din app, välj kontotyp och ange en omdirigerings-URL. Klicka sedan på **[!UICONTROL Register]** längst ned på sidan.

   ![](assets/five.png)

1. Du bör nu se din app på fliken **[!UICONTROL App registrations]**.

   ![](assets/six.png)

## Konfigurera programbehörigheter {#configuring-app-permissions}

1. Klicka på det program du vill konfigurera behörigheter för på fliken **[!UICONTROL App registrations]** i din Active Directory.

   ![](assets/seven.png)

1. Klicka på [!UICONTROL Manage] under **[!UICONTROL API permissions]**.

   ![](assets/eight.png)

1. Klicka på knappen **[!UICONTROL Add a permission]**.

   ![](assets/nine.png)

1. Välj **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Markera rutan **[!UICONTROL Access Common Data Service as organization users]** och klicka sedan på **[!UICONTROL Add permissions].**

   ![](assets/eleven.png)

1. När behörigheterna har lagts till, vänta minst 10 sekunder.

   ![](assets/twelve.png)

1. Klicka på knappen **[!UICONTROL Grant admin consent]**.

   ![](assets/thirteen.png)

1. Bekräfta genom att klicka på **[!UICONTROL Yes]**.

   ![](assets/fourteen.png)

   Och du är klar!

   ![](assets/fifteen.png)
