---
title: Arbeta med Experience Manager Assets
description: Lär dig hur du kan använda bildresurser från en ansluten AEM Assets-databas när du redigerar innehåll i Adobe Marketo Engage.
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Arbeta med resurser i Experience Manager

När Adobe Experience Manager Assets as a Cloud Service är integrerat med Adobe Marketo Engage blir det enkelt att upptäcka och få tillgång till digitala resurser som kan användas i ert marknadsföringsmaterial. När du redigerar ditt innehåll är resurserna tillgängliga från objektet _[!UICONTROL Assets]_i den vänstra navigeringen och när du redigerar e-postinnehåll för en kontoresa. Du kan också överföra resurser till en ansluten AEM Assets as a Cloud Service-databas direkt från Adobe Journey Optimizer B2B edition.

>[!NOTE]
>
>För närvarande stöds endast bildresurser från Adobe Experience Manager Assets i Adobe Journey Optimizer B2B edition. Ändringar av mediefilerna måste göras från Adobe Experience Manager Assets centrala arkiv. [Läs mer](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

När du använder dessa digitala resurser sprids de senaste förändringarna i Assets as a Cloud Service automatiskt till aktiva e-postkampanjer via länkade referenser. Om bilder tas bort i Adobe Experience Manager Assets as a Cloud Service visas bilderna med en bruten referens i e-postmeddelandena. När resurser som för närvarande används på kontoresor ändras eller tas bort, meddelas författarna av resan om bildändringarna och listan över resor som använder bilden. Alla ändringar av materialet måste göras i Adobe Experience Manager Assets centrala arkiv.

## Använd AEM Assets som bildkälla

Om din miljö har en eller flera databasanslutningar från Assets kan du ange AEM Assets som källa för resurser när du skapar eller visar information för ett e-postmeddelande, en e-postmall eller ett visuellt fragment.

* När du skapar ett nytt innehåll väljer du `AEM Assets` som **[!UICONTROL Image Source]**-objekt i dialogrutan.

SCREENSHOT

* När du öppnar en befintlig innehållsresurs väljer du `AEM Assets` på panelen _[!UICONTROL Body]_till höger.

SCREENSHOT

## Få åtkomst till resurser för redigering

>[!IMPORTANT]
>
>En administratör måste lägga till användare som behöver tillgång till Assets i produktprofilerna Assets Consumer Users eller/och Assets Users. [Läs mer](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

Klicka på ikonen _Resursväljare_ i den vänstra sidofältet i den visuella innehållsredigeraren. Detta ändrar verktygspanelen till en lista med tillgängliga resurser i den valda databasen.

SCREENSHOT

Om du har fler än en ansluten AEM databaser klickar du på menypilen för **[!UICONTROL Repository]** för att välja den databas som du vill använda.

SCREENSHOT

Det finns flera metoder för att lägga till en bildresurs på den visuella arbetsytan:

* Dra och släpp en miniatyrbild från den vänstra navigeringen.

SCREENSHOT

* Lägg till en bildkomponent på arbetsytan och klicka på **[!UICONTROL Browse]** för att öppna dialogrutan _[!UICONTROL Select Assets]_.

  I dialogrutan kan du välja en bild från den valda databasen.

  Det finns flera verktyg som hjälper dig att hitta den resurs du behöver.

SCREENSHOT

* Ändra **[!UICONTROL Repository]** överst till höger.

* Klicka på **[!UICONTROL Manage assets]** överst till höger för att öppna Assets-databasen på en annan webbläsarflik och använda AEM Assets hanteringsverktyg.

* Klicka på _vytypsväljaren_ längst upp till höger för att ändra visningen till **[!UICONTROL List View]**, **[!UICONTROL Grid View]**, **[!UICONTROL Gallery View]** eller **[!UICONTROL Waterfall View]**.

* Klicka på ikonen _Sorteringsordning_ om du vill ändra sorteringsordningen mellan stigande och fallande.

* Klicka på menypilen **[!UICONTROL Sort by]** om du vill ändra sorteringsvillkoren till **[!UICONTROL Name]**, **[!UICONTROL Size]** eller **[!UICONTROL Modified]**.

* Klicka på ikonen _Filter_ längst upp till vänster om du vill filtrera de visade objekten enligt dina kriterier.

* Ange text i sökfältet för att filtrera de visade objekten så att de matchar resursnamnet.

SCREENSHOT
