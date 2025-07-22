---
unique-page-id: 2359798
description: Lägg till fler CNAME-filer för landningssida - Marketo Docs - produktdokumentation
title: Lägg till ytterligare CNAME för landningssida
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Lägg till ytterligare CNAME för landningssida {#add-additional-landing-page-cnames}

Du kanske vill lägga till CNAME för landningssidor så att olika URL:er kan peka mot Marketo landningssidor. Om du följer stegen nedan kan du hantera flera domäner.

>[!CAUTION]
>
>Cookies kan inte delas mellan domäner.

>[!TIP]
>
>**Samma toppnivådomän - bra! Cookies delas**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**Olika toppnivådomäner - Felaktiga! Cookies är _inte_ delade**.<br/> kör.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Klicka på **Mitt konto**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Bläddra ned till &quot;Support Information&quot; och kopiera ditt Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Skicka begäran till IT {#send-request-to-it}

1. Be din IT-avdelning att installera följande CNAME: (Ersätt ordet [CNAME] med valfritt CNAME och [Munchkin ID] med texten från föregående steg).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Lägg till en ny CNAME {#add-a-new-cname}

1. Gå till **Admin** när IT-avdelningen har skapat CNAME.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Klicka på **Landningssidor**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Klicka på **[!UICONTROL New]** och välj sedan **[!UICONTROL New Domain Alias]**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Ange din **[!UICONTROL Domain Alias].** **[!UICONTROL Default Page]** visas om besökaren inte anger en URL. Ange vart de ska gå i så fall.

   >[!NOTE]
   >
   >För [!UICONTROL Default Page] kan du välja en landningssida eller en extern URL, till exempel din offentliga webbplats.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Ange din **[!UICONTROL Default Page]** och klicka på **[!UICONTROL Create]**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Snyggt! Nu vet du vad du ska göra om du någonsin vill lägga till en CNAME.
