---
unique-page-id: 15695874
description: Anslut [!DNL BrightTALK] till Marketo - Marketo Docs - produktdokumentation
title: Anslut [!DNL BrightTALK] till Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Anslut [!DNL BrightTALK] till Marketo {#connect-brighttalk-to-marketo}

Lär dig hur du ansluter din [!DNL BrightTALK]-kanal till din Marketo-instans. För att kunna göra detta måste du vara administratör för båda.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Steg i [!DNL BrightTALK] {#steps-in-brighttalk}

1. Logga in på [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} och klicka på **[!UICONTROL Connect Now]**.
1. Klicka på **[!UICONTROL Connect]** under [!UICONTROL Advanced Marketo Connector].
1. Du kommer till inloggningsskärmen och frågar efter: Klient-ID, Klienthemlighet, URL för identitetstjänst och URL för återställningstjänst. Logga in på Marketo för att få den här informationen.

## Steg i Marketo {#steps-in-marketo}

>[!NOTE]
>
>Nu måste du konfigurera [!DNL API Only User Role] och [!DNL API User] för att kunna begränsa vilka behörigheter [!DNL BrightTALK] har i din Marketo-instans. Eftersom vi redan har artiklar för de stegen länkar vi dig till dem.

1. Skapa en [API-roll endast för användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"} med API-rollen [!DNL BrightTALK] som du skapade under steg 4.

1. Gå tillbaka till området **[!UICONTROL Admin]**.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Klicka på **[!UICONTROL LaunchPoint]** under **[!UICONTROL Integration]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL New Service]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Ange ett **[!UICONTROL Display Name]** som du vill använda. Klicka på listrutan **[!UICONTROL Service]** och välj **[!UICONTROL Custom]** (markera _inte_ [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Kom ihåg att inte markera [!DNL BrightTALK] i listrutan. Det är ett fält som vi håller på att ta bort och om du väljer det kan det skapa betydande problem med din [!DNL Marketo/BrightTALK]-integrering.

1. Ange ett [!UICONTROL Description] som du vill använda. Klicka på listrutan **[!UICONTROL API Only User]** och välj [!DNL BrightTALK API User] som du skapade under steg 5. Klicka på **[!UICONTROL Create]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Klicka på **[!UICONTROL View Details]** för den anpassade tjänst du just skapade.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Kopiera och spara **[!UICONTROL Client ID]** och **[!UICONTROL Client Secret]**. Klicka på **[!UICONTROL Close]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Välj **[!UICONTROL Web Services]** under **[!UICONTROL Integration]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Under **[!UICONTROL Rest API]** kopierar (och sparar) du **[!UICONTROL Endpoint]** och **[!UICONTROL Identity]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Ytterligare steg i [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Gå tillbaka till konfigurationsskärmen för [!DNL BrightTALK]-anslutningen från steg 3 och ange de autentiseringsuppgifter som du sparade från steg 12 och 14.

När autentiseringsuppgifterna har autentiserats har du anslutit [!DNL BrightTALK] officiellt till Marketo. Nästa steg är att avgöra vilka datafält du vill synkronisera. Om du behöver hjälp med det kontaktar du supporten på [BrightTALK](https://www.brighttalk.com/){target="_blank"}.
