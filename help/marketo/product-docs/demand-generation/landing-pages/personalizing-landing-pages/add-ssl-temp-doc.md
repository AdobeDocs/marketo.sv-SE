---
description: Lägg till SSL på era landningssidor - Marketo Docs - produktdokumentation
title: Lägg till SSL på era landningssidor
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: 0e73866a4187d7bff67ce199e8d01e55081bcbef
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Lägg till SSL på era landningssidor {#add-ssl-to-your-landing-pages}

Lär dig att lägga till din varumärkesdomäns alias (t.ex. `http://business.adobe.com`) till landningssidor som skapats i Marketo Engage så att de kan nås under sina varumärkesdomäner.

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

## Aktivera SSL för din standarddomän

SCREENSHOT

>[!NOTE]
>
>* Kolumnen SSL-certifikat i listan visar certifikatstatus för alla domänalias som skapas efter att den här funktionen har släppts (DATE). Om SSL har aktiverats för en domän via Marketo Support finns certifikatet kvar, men visas inte i tabellen. Den här tabellen visar endast SSL-certifikat för domäner som lagts till med stegen i den här artikeln.
>
>* Det kan ta upp till tre minuter innan SSL är i READY-läge. Du måste uppdatera sidan för att ändringarna ska visas.
