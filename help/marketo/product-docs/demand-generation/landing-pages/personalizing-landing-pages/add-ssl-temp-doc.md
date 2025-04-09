---
description: Lägg till SSL på era landningssidor - Marketo Docs - produktdokumentation
title: Lägg till SSL på era landningssidor
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Lägg till SSL på era landningssidor {#add-ssl-to-your-landing-pages}

Med SSL-kryptering (Secure Socket Layer) kan du göra alla dina landningssidor för en Marketo Engage-instans säkra.

När du fyller i ett webbformulär eller besöker en landningssida som hanteras av Marketo Engage, skickas informationen som standard via ett osäkert protokoll (HTTP). Enligt företagets policy kanske du vill skydda den information som skickas till Marketo via HTTPS. När du till exempel besöker `http://info.mydomain.com/` blir det nu `https://info.mydomain.com/`.

Marketo Engage spårar &quot;Besökt webbsida&quot; och &quot;Klicka på länk på webbsida&quot; som standard över osäkra HTTP-protokoll. Om du vill att dina spårningslänkar ska vara skyddade med deras egna certifikat måste du ha Marketo som en separat icke-delad server för att kunna aktivera den. För att skydda alla aspekter av en kontakts interaktion med dig måste du vanligtvis skydda både landningssidor och spårningslänkar.

SCREENSHOT

## Aktivera SSL-certifiering {#enable-ssl-certification}

Lägg automatiskt till SSL för alla domänalias som du skapar som en del av reglerna för landningssidan.

1. Gå till området **Admin**.

   SCREENSHOT

1. Välj **Landningssidor** i trädet. Klicka på listrutan **Nytt** på fliken **Regler** och välj **Nytt domänalias**.

   SCREENSHOT

1. Markera kryssrutan **Skapa SSL-certifikat**.

   SCREENSHOT

Detta lägger automatiskt till ett SSL-certifikat för den här domänen.

SCREENSHOT

## Aktivera SSL för din standarddomän {#enable-ssl-default-domain}

SCREENSHOT

>[!NOTE]
>
>* Kolumnen SSL-certifikat i listan visar certifikatstatus för alla domänalias som skapas efter att den här funktionen har släppts (DATE). Om SSL har aktiverats för en domän via Marketo Support finns certifikatet kvar, men visas inte i tabellen. Den här tabellen visar endast SSL-certifikat för domäner som lagts till med stegen i den här artikeln.
>
>* Det kan ta upp till tre minuter innan SSL är i READY-läge. Du måste uppdatera sidan för att ändringarna ska visas.
