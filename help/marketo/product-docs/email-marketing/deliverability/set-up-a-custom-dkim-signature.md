---
unique-page-id: 2360219
description: Konfigurera en anpassad DKIM-signatur - Marketo Docs - Produktdokumentation
title: Konfigurera en anpassad DKIM-signatur
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Konfigurera en anpassad DKIM-signatur {#set-up-a-custom-dkim-signature}

För att säkerställa avancerad leverans signerar vi automatiskt all utgående e-post med en delad Marketo DKIM-signatur.

>[!NOTE]
>
>Du kan behöva hjälp av IT-avdelningen för att slutföra några av stegen i den här artikeln.

Du kan anpassa DKIM-signaturen så att den återspeglar de domäner du väljer. Så här gör du.

1. Gå till avsnittet **Admin** .

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >
   >Om du skapar en anpassad DKIM-signatur på det gammaldags sättet kommer den att fortsätta att fungera och visas här.

1. Klicka på **E-post**, sedan på fliken **DKIM** och slutligen **Lägg till domän**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Ange den domän du vill använda i Marketo-e-postmeddelanden som Från-adress och klicka på **Lägg till**.

   >[!TIP]
   >
   >
   >Om du använder en annan domän i din Från-adress använder vi Marketo-signaturen för DKIM.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Skicka **värdposten** och **TXT-värdet** till din IT-avdelning. Be dem att skapa posten åt dig och se till att den sprids till alla namnservrar som är kopplade till Från-domänen. Marketos DKIM-verifiering kräver att DKIM-nyckeln sprids till alla namnservrar som är associerade med den domän som DKIM-signerar.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. När de har bekräftat att de har skapat posten går de tillbaka till Marketo, väljer din domän och klickar på **Kontrollera DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Om bekräftelsen misslyckas och din IT-avdelning har skapat posten korrekt kan det bero på DNS-spridning. Försök igen senare.

   >[!CAUTION]
   >
   >
   >Om du ändrar/tar bort motsvarande DNS-post blir slutresultatet sämre. Se till att du tar bort posten i Marketo innan du gör DNS-ändringar.

   Detta är till stor hjälp när det gäller e-postleveransen. Du bör få en validering av att posten finns där och rätt.

