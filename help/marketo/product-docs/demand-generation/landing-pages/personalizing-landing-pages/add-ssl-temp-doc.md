---
description: Lägg till SSL på era landningssidor - Marketo Docs - produktdokumentation
title: Lägg till SSL på era landningssidor
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: f41d0595db695fc485a209aa2f9646a76e57acdf
workflow-type: tm+mt
source-wordcount: '199'
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

OBS:

SSL-certifikatskolumnen i listan visar SSL-certifikatstatus för alla domänalias som skapas efter att den här funktionen har släppts. Om SSL har aktiverats för en domän via stöd finns det fortfarande respektive SSL-certifikat, men tabellen visar endast SSL-certifikat för domäner som lagts till med den här funktionen

Det kan ta upp till 3 minuter för SSL att vara i READY-läge, och sidan måste uppdateras för att ändringar ska kunna spridas i användargränssnittet.
