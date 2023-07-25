---
unique-page-id: 2359798
description: Lägg till fler CNAME-filer för landningssida - Marketo Docs - produktdokumentation
title: Lägg till ytterligare CNAME för landningssida
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Lägg till ytterligare CNAME för landningssida {#add-additional-landing-page-cnames}

Du kanske vill lägga till CNAME för landningssidor så att olika URL:er kan peka mot Marketo landningssidor. Om du följer stegen nedan kan du hantera flera domäner.

>[!CAUTION]
>
>Cookies kan inte delas mellan domäner.

>[!TIP]
>
>**Samma toppnivådomän - bra! Cookies delas**.<br/> **go**.mincompany.com > **info**.mincompany.com
>
>**Olika toppnivådomäner - Felaktiga! Cookies är _not_ delad**.<br/> gå.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Administratör** område.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Klicka **Mitt konto**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Bläddra ned till &quot;Support Information&quot; och kopiera ditt Munchkin-ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Skicka begäran till IT {#send-request-to-it}

1. Be din IT-avdelning att installera följande CNAME: (Ersätt ordet [CNAME] med valfri CNAME och [Munchkin-ID] med texten från föregående steg).

   [CNAME].YourCompany.com > [Munchkin-ID].mktoweb.com

## Lägg till en ny CNAME {#add-a-new-cname}

1. När IT-avdelningen har skapat CNAME går du till **Administratör** område.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Klicka **Landningssidor**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Klicka **Nytt** välj **Nytt domänalias**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Ange **Domänalias.** The **Standardsida** visas om besökaren inte anger en URL. Ange vart de ska gå i så fall.

   >[!NOTE]
   >
   >För standardsidan kan du välja en landningssida eller en extern URL-adress, till exempel din offentliga webbplats.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Ange **Standardsida** och klicka **Skapa**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Snyggt! Nu vet du vad du ska göra om du någonsin vill lägga till en CNAME.
