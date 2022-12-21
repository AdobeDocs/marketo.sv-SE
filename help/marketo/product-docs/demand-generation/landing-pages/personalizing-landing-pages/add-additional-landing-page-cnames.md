---
unique-page-id: 2359798
description: Lägg till fler CNAME-filer för landningssida - Marketo Docs - produktdokumentation
title: Lägg till ytterligare CNAME för landningssida
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
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

## Hitta din kontosträng {#find-your-account-string}

1. Gå till **Administratör** område och klicka **Landningssidor**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Kopiera **Kontosträng** från **Inställningar** -avsnitt.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Anteckna det för nästa steg.

## Skicka begäran till IT {#send-request-to-it}

1. Be din IT-avdelning att installera följande CNAME: (Ersätt ordet [CNAME] med valfri CNAME och [KONTOSTRÄNG] med texten från föregående steg).

   [CNAME].YourCompany.com > [KONTOSTRÄNG].mktoweb.com

## Lägg till en ny CNAME {#add-a-new-cname}

1. När IT-avdelningen har skapat CNAME går du till **Administratör** sedan klicka **Landningssidor**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Klicka **Nytt** välj **Nytt domänalias**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Ange **Domänalias.** The **Standardsida** visas om besökaren inte anger en URL. Ange vart de ska gå i så fall.

   >[!NOTE]
   >
   >För standardsidan kan du välja en landningssida eller en extern URL-adress, till exempel din offentliga webbplats.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Ange **Standardsida** och klicka **Skapa**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Snyggt! Nu vet du vad du ska göra om du någonsin vill lägga till en CNAME.
