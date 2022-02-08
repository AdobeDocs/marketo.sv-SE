---
unique-page-id: 37356194
description: Skicka en lista till Adobe Experience Cloud - Marketo Docs - produktdokumentation
title: Skicka en lista till Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
source-git-commit: a82a2dd0a9c3a27b9b6bf3b352cd81d59932a31b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Skicka en lista till Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>En HIPAA-klar distribution av en Marketo-instans kan inte använda den här funktionen.

>[!PREREQUISITES]
>
>[Konfigurera Adobe Experience Cloud målgruppsdelning](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Målprogram som stöds {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (**endast** om du äger en Adobe Audience Manager-licens)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## Skicka en statisk lista {#how-to-send-a-static-list}

En statisk lista är bara det, statiskt. Listan i Adobe Experience Cloud ändras inte om du inte gör det manuellt.

1. I Marketo hittar du den lista du vill exportera. Högerklicka på den och välj **Skicka till Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Klicka på **Audience Manager** och markera önskad målmapp i Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Välj om du vill skapa en ny målgrupp eller skriva över en befintlig (i det här exemplet skapar vi en ny). Ange det nya målgruppsnamnet och klicka på **Skicka**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Klicka **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >Det kan ta upp till 6-8 timmar för publiken att bli fullt utnyttjad i Adobe.

## Skicka en synkroniserad lista {#how-to-send-a-synced-list}

Synkronisering av en lista innebär att när du uppdaterar en lista i Marketo synkroniseras ändringen automatiskt med målgruppen i Adobe Experience Cloud.

1. I Marketo hittar du den lista du vill exportera. Högerklicka på den och välj **Skicka till Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Klicka på **Målbiblioteksmapp** och markera önskad målmapp i Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Välj om du vill skapa en ny målgrupp eller skriva över en befintlig (i det här exemplet skapar vi en ny). Ange det nya målgruppsnamnet, kontrollera **Håll målgruppsmedlemskapet synkat** och klicka **Skicka**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Klicka **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Stoppa listsynkronisering {#how-to-stop-a-list-sync}

Du kan när som helst stoppa synkroniseringen av listan.

1. I Marketo söker du efter och högerklickar på den lista som du vill sluta synkronisera. Klicka **Synkronisering av stopplista**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Markera de målgrupper som du vill sluta synkronisera och klicka på **Stoppa**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Klicka **Stoppa** för att bekräfta.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Saker att notera {#things-to-note}

**Dela till Adobe Analytics**

För kunder som äger både Adobe Audience Manager och Adobe Analytics kommer denna integrering att göra det möjligt att dela målgrupper från Marketo till Adobe Analytics Report Suites, men det finns några ytterligare konfigurationsåtgärder som måste vidtas i Adobe Audience Manager för att detta ska vara möjligt. Läs Adobe Audience Manager dokumentation om du vill veta mer om hur du konfigurerar detta: [https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Trait Usage för Adobe Audience Manager-kunder**

När du initierar en listexport i Marketo kommer du att märka att följande ändringar återspeglas i din Adobe Audience Manager-instans:

* För alla leads i den exporterade listan skriver Marketo ett spår med Leads hashade e-postmeddelanden som en enhetsidentifierare. Namnet på egenskapen matchar målpublikens namn som du angav under exporten.
* För alla ECID:n som Marketo har lyckats matcha med Leads i den exporterade listan skriver Marketo ett spår med ECID-enhetsidentifieraren. Namnet på egenskapen matchar målpublikens namn som du angav under exporten.
* Marketo kommer också att skapa ett segment i din Audience Manager Instance med ECID-egenskapen som det enda segmenteringskriteriet. Segmentets namn matchar målpublikens namn som du angav under exporten.

## Vanliga frågor {#faq}

**Varför skiljer sig liststorleken i Marketo från den i Adobe?**

Under huven fungerar målgruppsintegreringen genom att synkronisera Marketo Munchkin-cookies med motsvarande Adobe ECID-cookie. Marketo kan bara dela medlemskapsdata för leads som Marketo har synkroniserat ett ECID för. För att få bästa möjliga resultat rekommenderar vi att du läser in Marketo munchkin.js-spårningsskript parallellt med Adobe&#39;s visitor.js tracking-kod på alla sidor som du är intresserad av att spåra i marknadsföringssyfte.

**Hur fungerar cookie-synkroniseringen?**

När synkroniseringen av cookies är aktiverad för din Marketo-prenumeration försöker Marketo munchkin.js att hämta och lagra ECID:n för Adobe för den Adobe IMS-organisation som du angav under integreringsinställningen och matcha dessa ECID:n med motsvarande Marketo cookie-identifierare. På så sätt kan Marketo anonyma användarprofiler berikas med ECID:n för Adobe.

Ytterligare ett steg krävs för att koppla den anonyma användarprofilen till en lead-profil, som identifieras med ett enkelt textmeddelande. Exakt hur detta fungerar [beskrivs här](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Vilken information delas?**

Den här integreringen delar bara information om medlemskap från Marketo till Adobe (t.ex. kunskap om att Lead X är medlem i List Y). Inga ytterligare leadattribut delas till Adobe via den här integreringen.
