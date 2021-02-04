---
unique-page-id: 2359798
description: Lägg till fler CNAME-filer för landningssida - Marketo Docs - Produktdokumentation
title: Lägg till ytterligare CNAME för landningssida
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Lägg till ytterligare CNAME för landningssida {#add-additional-landing-page-cnames}

Du kanske vill lägga till CNAME för landningssidor så att olika URL:er kan peka mot era Marketo-landningssidor. Om du följer stegen nedan kan du hantera flera domäner.

>[!CAUTION]
>
>Cookies kan inte delas mellan domäner.

>[!TIP]
>
>**Samma toppnivådomän - bra! Cookies delas**.<br/> **go**.mycompany.com >  **info**.mycompany.com
>
>**Olika toppnivådomäner - Felaktiga! Cookies är _inte_ delade**.<br/> gå.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Hitta din kontosträng {#find-your-account-string}

1. Gå till området **Admin** och klicka på **Startsidor**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Kopiera **kontosträngen** från avsnittet **Inställningar**.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Anteckna det för nästa steg.

## Skicka begäran till IT {#send-request-to-it}

1. Be din IT-avdelning att installera följande CNAME: (Ersätt ordet [CNAME] med valfritt CNAME och [KONTOSTRING] med texten från föregående steg).

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## Lägg till en ny CNAME {#add-a-new-cname}

1. När IT-avdelningen har skapat CNAME går du till **Admin** och klickar sedan på **Landing Pages**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Klicka på **Nytt** och välj sedan **Nytt domänalias**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Ange ditt **domänalias.** Standardsidan  **** visas om besökaren inte anger någon URL. Ange vart de ska gå i så fall.

   >[!NOTE]
   >
   >För standardsidan kan du välja en landningssida eller en extern URL-adress, till exempel din offentliga webbplats.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Ange din **standardsida** och klicka på **Skapa**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Snyggt! Nu vet du vad du ska göra om du någonsin vill lägga till en CNAME.
