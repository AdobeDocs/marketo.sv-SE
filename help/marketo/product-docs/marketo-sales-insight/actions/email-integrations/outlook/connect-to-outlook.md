---
description: Anslut till Outlook - Marketo Docs - produktdokumentation
title: Anslut till Outlook
exl-id: 760db2d2-2e5d-4988-891a-9c57250264ac
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Anslut till Outlook {#connect-to-outlook}

Lär dig hur du ansluter kontot Sales Insight Actions till Outlook.

>[!NOTE]
>
>Varje användare måste ansluta till Outlook från sitt Marketo-försäljningskonto.

## Ansluter till Outlook Online {#connecting-to-outlook-online}

Att ansluta till Outlook innebär att du får svarsspårning, åtkomst till leveranskanalen i Outlook, möjlighet att schemalägga e-postmeddelanden i Outlook och skicka regelefterlevnad.

1. Klicka på kugghjulsikonen i Marketo Sales och välj **Settings**.

   ![](assets/connect-to-outlook-1.png)

1. Välj **E-postinställningar** under Mitt konto.

   ![](assets/connect-to-outlook-2.png)

1. Klicka på fliken **E-postanslutning**.

   ![](assets/connect-to-outlook-3.png)

1. Klicka på **Kom igång**.

   ![](assets/connect-to-outlook-4.png)

1. Välj **Jag använder Outlook för att skicka e-post** och klicka på **Nästa**.

   ![](assets/connect-to-outlook-5.png)

1. Markera den version av Outlook som du använder och klicka på **Nästa**. I det här exemplet väljer vi Outlook Online.

   ![](assets/connect-to-outlook-6.png)

   <table>
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td>
      <td>Kallas även Exchange Online</td>
     </tr>
     <tr>
      <td><strong>Lokal Exchange</strong></td>
      <td>Inkluderar Exchange 2013 och 2016</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Marketo stöder för närvarande inte hybridkonton i Exchange.

1. Klicka på **OK**.

   ![](assets/connect-to-outlook-7.png)

1. Om du inte är inloggad i Outlook anger du din inloggningsinformation och klickar på **Nästa**. Om du är det väljer du det konto du vill ansluta till och klickar på **Nästa**. I det här exemplet är vi redan inloggade.

   ![](assets/connect-to-outlook-8.png)

1. Klicka på **Acceptera**.

   ![](assets/connect-to-outlook-9.png)

   Du kan använda den här anslutningen för att spåra e-postmeddelanden och även som en leveranskanal.

   >[!NOTE]
   >
   >Outlook Online (Office365) tillämpar sina egna sändningsbegränsningar. [Läs mer här](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## Ansluter till Exchange On-Premise {#connecting-to-exchange-on-premise}

Att ansluta till Exchange On-Premise innebär att du får svarsspårning, åtkomst till Outlooks leveranskanal, möjlighet att schemalägga e-postmeddelanden i Outlook och skicka regelefterlevnad.

1. Klicka på kugghjulsikonen i Marketo Sales och välj **Settings**.

   ![](assets/connect-to-outlook-10.png)

1. Välj **E-postinställningar** under Mitt konto.

   ![](assets/connect-to-outlook-11.png)

1. Klicka på fliken **E-postanslutning**.

   ![](assets/connect-to-outlook-12.png)

1. Klicka på **Kom igång**.

   ![](assets/connect-to-outlook-13.png)

1. Välj **Jag använder Outlook för att skicka e-post** och klicka på **Nästa**.

   ![](assets/connect-to-outlook-14.png)

1. Markera den version av Outlook som du använder och klicka på **Nästa**. I det här exemplet väljer vi Exchange On-Local.

   ![](assets/connect-to-outlook-15.png)

   <table>
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td>
      <td>Kallas även Exchange Online</td>
     </tr>
     <tr>
      <td><strong>Lokal Exchange</strong></td>
      <td>Inkluderar Exchange 2013 och 2016</td>
     </tr>
    </tbody>
   </table>

1. Ange dina autentiseringsuppgifter och klicka på **Anslut**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >Om du stänger av Automatisk upptäckt i listrutan Exchange-version måste du fråga din IT-avdelning om Exchange-URL:en.

   Du kan använda den här anslutningen för att spåra e-postmeddelanden och även som en leveranskanal.

   >[!NOTE]
   >
   >När du använder Exchange On-prem fastställer IT-teamet din sändningsgräns för e-post.

## Hämtar behörighet att ansluta till Outlook Online {#getting-permission-to-connect-to-outlook-online}

Du kan behöva samarbeta med IT-avdelningen för att få tillstånd att tillåta Marketo Sales att ansluta till ditt Outlook Online-konto (Microsoft 365).

>[!NOTE]
>
>Informera IT-avdelningen som hanterar ditt Microsoft 365-konto om att programmet som behöver åtkomst är&quot;Marketo Sales Connect&quot;.

Beroende på ditt IT-teams önskemål och aktuella konfiguration är det bäst att rådfråga dem om hur de ska bevilja åtkomst. Nedan finns några artiklar som kan vägleda konversationen.

* Global samtycke: [Integrerade appar och Azure AD för Microsoft 365-administratörer](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* Användarsamtycke: [Konfigurera hur användare godkänner program](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&pivots=portal){target="_blank"}
* Administratörssamtycke: [Konfigurera arbetsflödet för administratörsgodkännande](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&view=o365-worldwide){target="_blank"}
* Aktivera eller inaktivera användargodkännande: [Hantera användargodkännande för appar i Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&view=o365-worldwide){target="_blank"}
* Hantera med Microsoft Defender: [Hantera OAuth-appar](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
