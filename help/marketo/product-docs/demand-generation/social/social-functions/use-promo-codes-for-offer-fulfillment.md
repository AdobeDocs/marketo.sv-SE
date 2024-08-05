---
unique-page-id: 2359819
description: Använd kampanjkoder för att fylla i erbjudanden - Marketo Docs - produktdokumentation
title: Använd kampanjkoder för att slutföra erbjudandet
exl-id: 71cfc1c5-ecd3-435f-8c8c-1a93478fe80c
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Använd kampanjkoder för att slutföra erbjudandet {#use-promo-codes-for-offer-fulfillment}

När du skapar ett hänvisningserbjudande eller en utlottning kan du skicka en kampanjkod till varje vinnare. För att lösa in belöningen använder de koden, till exempel på utcheckningssidan för ett köp på din webbplats.

>[!IMPORTANT]
>
>Den 31 juli 2024 började vi ta bort den här funktionen. Nya resurser kan inte längre skapas. Befintliga tillgångar kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Ladda upp kampanjkoder {#upload-promo-codes}

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-2.png)

1. Markera hänvisningserbjudandet och klicka på **Redigera utkast**.

   ![](assets/image2015-4-22-11-3a16-3a45.png)

1. Gå till **Appinställningar** och sedan till **Erbjudandeinformation** i redigeraren för hänvisningserbjudanden.

   ![](assets/image2015-4-22-11-3a23-3a39.png)

1. Under E-post väljer du **Använd kampanjkoder** och under Överför koder klickar du på **Bläddra** för att välja kampanjkodsfilen i systemet.

   ![](assets/image2015-4-22-12-3a52-3a43.png)

1. Kampanjkodsfilen måste vara en vanlig ASCII-textfil med en kod per rad och ett .txt-filnamnstillägg. Exempel:

   ![](assets/image2015-4-22-13-3a2-3a23.png)

   >[!CAUTION]
   >
   >Allt tomt utrymme i kampanjkodsfilen behandlas som en del av koden på den raden. Var särskilt försiktig så att du undviker efterföljande blanksteg i slutet av varje rad.

1. När överföringen är klar visas det totala antalet överförda koder.

   ![](assets/image2015-4-22-13-3a8-3a31.png)

## Granska skickade kampanjkoder {#review-sent-promo-codes}

När deltagarna har börjat tjäna på erbjudandet ser du vilka kampanjkoder som skickats till vem och när.

>[!NOTE]
>
>Endast Marketo-användare med _Access Awards_-behörighet har åtkomst till den här informationen. Se [Hantera användarroller och behörigheter](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-2.png)

1. Välj ditt hänvisningserbjudande eller utlottningar och klicka på fliken **Deltagare**.

   ![](assets/image2015-4-22-11-3a36-3a22.png)

1. Här ser du några tävlingsbidrag. Klicka på siffran i kolumnen **Promo Codes** för att se kampanjkoderna som skickades till deltagaren och när.

   ![](assets/image2015-4-22-11-3a36-3a43.png)
