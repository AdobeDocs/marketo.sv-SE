---
description: Konfigurera din Marketo-anslutning manuellt - Marketo Docs - Produktdokumentation
title: Konfigurera din Marketo-anslutning manuellt
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Konfigurera din Marketo-anslutning manuellt {#manually-set-up-your-marketo-connection}

>[!NOTE]
>
>När du etablerar MSC skickar Marketo automatiskt dina inloggningsuppgifter till Sales Connect och ansluter instansen till Marketo. Det här steget krävs **endast** om du inte ser anslutningen som upprättats efter att din Sales Connect-instans har etablerats. Om anslutningen är upprättad ser du dina inloggningsuppgifter på sidan Marketo Admin Settings.

## Hämtar autentiseringsuppgifter innan du ansluter försäljningen Anslut till Marketo {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Du måste hämta en uppsättning inloggningsuppgifter inifrån Marketo. Dessa autentiseringsuppgifter används senare av Sales Connect Admin för att ansluta Marketo till Sales Connect.

1. Klicka på **Admin** i Marketo.

   ![](assets/manually-set-up-your-marketo-connection-1.png)

1. Klicka på **Sales Connect** i trädet.

   ![](assets/manually-set-up-your-marketo-connection-2.png)

1. Välj och skicka följande Marketo-autentiseringsuppgifter till din Sales Connect-administratör: Munchkin-ID, klient-ID, klienthemlighet.

   ![](assets/manually-set-up-your-marketo-connection-3.jpg)

   >[!NOTE]
   >
   >När du kopierar och klistrar in ovanstående information bör du kontrollera att inga mellanslag läggs till.

## Anslut försäljningsanslutning till Marketo {#connect-sales-connect-to-marketo}

1. Klicka på kugghjulsikonen i Sales Connect och välj **Inställningar**.

   ![](assets/manually-set-up-your-marketo-connection-4.png)

1. Under Administratörsinställningar väljer du **Marketo**.

   ![](assets/manually-set-up-your-marketo-connection-5.png)

1. Ange de Marketo-autentiseringsuppgifter som tillhandahålls av Marketo Admin och klicka på **Anslut**.

   ![](assets/manually-set-up-your-marketo-connection-6.png)
