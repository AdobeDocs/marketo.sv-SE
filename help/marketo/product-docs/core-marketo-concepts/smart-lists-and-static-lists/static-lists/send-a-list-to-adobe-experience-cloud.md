---
unique-page-id: 37356194
description: Skicka en lista till Adobe Experience Cloud - Marketo Docs - produktdokumentation
title: Skicka en lista till Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: 781f1350b4eae731bd77013ed9f238d77a6fcd32
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# Skicka en lista till Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>En HIPAA-klar distribution av en Marketo Engage-instans kan inte använda den här funktionen.

>[!PREREQUISITES]
>
>[Konfigurera Adobe organisationsmappning](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Målprogram som stöds {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_endast_ om du äger en Adobe Audience Manager-licens)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-Time Customer Data Platform
* Adobe Target

## Skicka en statisk lista {#how-to-send-a-static-list}

En statisk lista är bara det, statiskt. Listan i Adobe Experience Cloud ändras inte om du inte gör det manuellt.

1. I Marketo hittar du den lista som du vill exportera. Högerklicka på den och välj **[!UICONTROL Send to Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Klicka på listrutan **[!UICONTROL Audience Manager Folder]** och välj önskad målmapp i Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Välj om du vill skapa en ny målgrupp eller skriva över en befintlig (i det här exemplet skapar vi en ny). Ange det nya publiknamnet och klicka på **[!UICONTROL Send]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Klicka på **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >Det kan ta upp till 6-8 timmar för målgruppsmedlemskap att fullt ut fylla i Adobe.

## Skicka en synkroniserad lista {#how-to-send-a-synced-list}

Synkronisering av en lista innebär att när du uppdaterar en lista i Marketo synkroniseras ändringen automatiskt med målgruppen i Adobe Experience Cloud.

1. I Marketo hittar du den lista som du vill exportera. Högerklicka på den och välj **[!UICONTROL Send to Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Klicka på listrutan **[!UICONTROL Audience Library Folder]** och välj önskad målmapp i Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Välj om du vill skapa en ny målgrupp eller skriva över en befintlig (i det här exemplet skapar vi en ny). Ange det nya målgruppsnamnet, markera rutan **[!UICONTROL Keep Audience Membership in Sync]** och klicka på **[!UICONTROL Send]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Klicka på **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Stoppa listsynkronisering {#how-to-stop-a-list-sync}

Du kan när som helst stoppa synkroniseringen av listan.

1. I Marketo söker du efter och högerklickar på den lista som du vill sluta synkronisera. Klicka på **[!UICONTROL Stop List Sync]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Markera de målgrupper som du vill sluta synkronisera och klicka på **[!UICONTROL Stop]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Bekräfta genom att klicka på **[!UICONTROL Stop]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Saker att notera {#things-to-note}

### Dela till Adobe Analytics {#sharing-to-adobe-analytics}

* För användare som äger både Adobe Audience Manager och Adobe Analytics kommer denna integrering att göra det möjligt att dela målgrupper från Marketo till dina Adobe Analytics Report Suites, men det finns några ytterligare konfigurationsåtgärder som måste vidtas i Adobe Audience Manager för att detta ska vara möjligt. Mer information om hur du konfigurerar det här finns i [Adobe Audience Manager-dokumentationen](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=sv-SE){target="_blank"}.

* När en lista har överförts från Marketo till Adobe Audience Manager kan den även nås av Adobe Target. Konfigurationen [måste aktiveras i Adobe Target](https://experienceleague.adobe.com/sv/docs/target/using/integrate/audience-manager-target-integration){target="_blank"}.

* Om en lista är tom, eller inte har några personer med ECID-värden, skickas inte listnamnet för referens utanför Marketo.

### Trait Usage för Adobe Audience Manager-kunder {#trait-usage-aam}

När du initierar en listexport i Marketo kommer du att märka att följande ändringar återspeglas i din Adobe Audience Manager-instans:

* För alla personer i den exporterade listan skriver Marketo ett spår med hjälp av sina hash-kodade e-postmeddelanden som en identifierare för olika enheter. Namnet på egenskapen matchar målpublikens namn som du angav under exporten.
* För alla ECID:n som Marketo har lyckats matcha med personerna i den exporterade listan, kommer Marketo att skriva ett spår med ECID-enhetsidentifieraren. Namnet på egenskapen matchar målpublikens namn som du angav under exporten.
* Marketo kommer också att skapa ett segment i din Audience Manager Instance med ECID-egenskapen som det enda segmenteringskriteriet. Segmentets namn matchar målpublikens namn som du angav under exporten.

## Vanliga frågor och svar {#faq}

**Varför skiljer sig liststorleken i Marketo från den i Adobe?**

Under huven fungerar målgruppsintegreringen genom att synkronisera Marketo Munchkin-cookies med motsvarande Adobe ECID-cookie. Marketo kan bara dela medlemskapsdata för personer som Marketo har synkroniserat ett ECID för. För att få bästa möjliga resultat rekommenderar vi att du läser in spårningsskript för Marketo munchkin.js parallellt med spårningskoden för Adobe visitor.js på alla sidor som du är intresserad av att spåra i marknadsföringssyfte.

**Hur fungerar cookie-synkroniseringen?**

När synkroniseringen av cookies är aktiverad för din Marketo-prenumeration försöker Marketo munchkin.js hämta och lagra Adobe ECID:n för den Adobe IMS-organisation som du angav under integreringsinställningen och matcha dessa ECID:n med motsvarande Marketo cookie-identifierare. Detta gör att Marketo anonyma användarprofiler kan berikas med Adobe ECID:n.

Ytterligare ett steg krävs för att koppla den anonyma användarprofilen till en personprofil, som identifieras med ett vanligt textmeddelande. Exakt hur detta fungerar [beskrivs här](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Vilken information delas?**

Den här integreringen delar bara information om medlemskap från Marketo till Adobe (t.ex. kännedom om att person X är medlem i lista Y). Inga ytterligare personattribut delas till Adobe via den här integreringen.
