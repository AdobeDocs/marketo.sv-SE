---
unique-page-id: 1900589
description: Lägg till spårade länkar i ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Lägg till spårade länkar i ett e-postmeddelande
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Lägg till spårade länkar i ett e-postmeddelande {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [Skapa ett e-postmeddelande med endast text](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [Redigera element i ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

E-postlänkar med text kan spåras i Marketo. Låt oss se hur det fungerar.

1. Markera e-postmeddelandet och klicka på **Redigera utkast**.

1. Välj din e-postadress och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/one-9.png)

1. Dubbelklicka på det redigerbara området som du vill lägga till länken i.

   ![](assets/two-8.png)

1. Ange URL-adressen med dubbla hakparenteser, så här: `[[www.domain.com/path/page.html]]`.

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >Om ett e-postmeddelande skickades för över 365 dagar sedan **och** ingen har klickat på någon av länkarna de senaste 180 dagarna, rensar Marketo Engage vägen till URL:en från vår databas, vilket gör att länken bryts. Använd inte spärra/knip om du vill att länken ska vara permanent.

1. Stäng av redigeraren och glöm inte att godkänna utkastet.

   ![](assets/four-6.png)

>[!NOTE]
>
>Funktionen för klassen mktNoTok fungerar inte med spårbara länkar i textmeddelanden. Endast för HTML e-post.
