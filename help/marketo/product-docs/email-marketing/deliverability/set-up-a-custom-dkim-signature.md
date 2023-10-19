---
unique-page-id: 2360219
description: Konfigurera en anpassad DKIM-signatur - Marketo Docs - produktdokumentation
title: Konfigurera en anpassad DKIM-signatur
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 9e731fa02cd20b34f48c7f85241b97f4c507d4a9
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Konfigurera en anpassad DKIM-signatur {#set-up-a-custom-dkim-signature}

För att säkerställa avancerad leverans signerar vi automatiskt all utgående e-post med en delad Marketo DKIM-signatur.

>[!NOTE]
>
>Du kan behöva hjälp av IT-avdelningen för att slutföra några av stegen i den här artikeln.

Du kan anpassa DKIM-signaturen så att den återspeglar vilken eller vilka domäner du väljer. Så här gör du.

1. Gå till **Administratör** -avsnitt.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Om du skapar en anpassad DKIM-signatur på det gammaldags sättet kommer den att fortsätta att fungera och visas här.

1. Klicka **E-post**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1, Klicka på **SPF/DKIM** tabbtangenten, sedan **Lägg till domän**.

![](assets/set-up-a-custom-dkim-signature-3.png)

1. Ange den domän som du kommer att använda i Marketo e-postmeddelanden som Från-adress. Välj en väljare och en nyckelstorlek. Klicka **Lägg till** när det är klart.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   >[!TIP]
   >
   >* Vi rekommenderar nyckelstorleken 2048.
   >* Om du använder en annan domän i din Från-adress använder vi den Marketo delade DKIM-signaturen.

1. Skicka **Värdpost** och **TXT Value** till din IT-avdelning. Be dem att skapa posten åt dig och se till att den sprids till alla namnservrar som är kopplade till Från-domänen. Marketo DKIM-verifiering kräver att DKIM-nyckeln sprids till alla namnservrar som är associerade med den domän som DKIM-signerar.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. När de har bekräftat att de har skapat posten går du tillbaka till Marketo, väljer din domän och klickar på **Kontrollera DNS**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Om bekräftelsen misslyckas och din IT-avdelning har skapat posten korrekt kan det bero på DNS-spridning. Försök igen senare.

   >[!CAUTION]
   >
   >Om du ändrar/tar bort motsvarande DNS-post blir slutresultatet sämre. Se till att du tar bort posten i Marketo innan du gör DNS-ändringar.

   Detta är till stor hjälp när det gäller e-postleveransen. Du bör få en validering av att posten finns där och rätt.
