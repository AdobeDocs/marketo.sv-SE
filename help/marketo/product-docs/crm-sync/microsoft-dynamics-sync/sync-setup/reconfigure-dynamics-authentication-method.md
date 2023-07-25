---
description: Konfigurera om Dynamics-autentiseringsmetod - Marketo Docs - produktdokumentation
title: Konfigurera om Dynamics-autentiseringsmetod
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Konfigurera om Dynamics-autentiseringsmetod {#reconfigure-dynamics-authentication-method}

Följ stegen nedan för att uppdatera din Dynamics-autentiseringsmetod.

>[!PREREQUISITES]
>
>Konfigurera programmet i Microsoft Dynamics och den aktiva katalogen (Azure AD/ADFS) med önskad autentiseringsmetod från någon av följande artiklar:
>
>* [Steg 2 av 3: Konfigurera Marketo Solution med Server to Server Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [Steg 2 av 4: Konfigurera Marketo Solution med Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)

1. I Marketo klickar du **Administratör**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Klicka **Microsoft Dynamics** sedan **Inaktivera synkronisering**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Du måste inaktivera den globala synkroniseringen tillfälligt för att kunna uppdatera autentiseringsmetoden.

1. Klicka på **Konfigurera om ny autentiseringsmetod** -fliken.

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Välj önskad ny autentiseringsmetod (i det här exemplet väljer vi webb-API).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Ange de autentiseringsuppgifter som krävs för den nya autentiseringsmetoden och klicka på **Validera**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* De specifika fälten varierar beroende på vald autentiseringsmetod och formuläret uppdateras automatiskt beroende på föregående autentiseringsmetod.
   >* Om du har synkroniserat tidigare kan data i ovanstående formulär vara förifyllda. Ange alla inloggningsuppgifter igen för att säkerställa rätt värden.

1. Om allt är bra genereras alla gröna bockar i Validera synkronisering ![](assets/green-check.png). Granska meddelandet och klicka på **Byt** för att uppdatera autentiseringsmetoden.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Om du ser en ![](assets/red-x.png), det steget har ett problem. Se [Åtgärda problem med synkronisering av Dynamics-validering](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) för att identifiera och åtgärda problem. Kör sedan synkroniseringsvalideringsstegen igen tills resultatet ser ut som bilden ovan.

1. Klicka **Bekräfta** för att fortsätta.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Klicka **Bekräfta** igen.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Klicka **OK**.

   >[!IMPORTANT]
   >
   >Det tar 15 minuter att godkänna det nya autentiseringsläget. Vänta 15 minuter från switchtiden innan du aktiverar synkroniseringen igen.
