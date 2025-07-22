---
unique-page-id: 1147356
description: Understanding Email Event Logging - Marketo Docs - Product Documentation
title: E-posthändelseloggning
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# E-posthändelseloggning {#understanding-email-event-logging}

När du skickar e-post loggar Marketo olika datapunkter till personens aktivitetsloggar. Här är de grundläggande.

| Händelse | Beskrivning |
|---|---|
| [!UICONTROL Sent] | Loggas varje gång ett e-postmeddelande skickas från Marketo-servrarna, oavsett om det faktiskt skickas. Studsade e-postmeddelanden loggas fortfarande som&quot;Skickat&quot;. |
| [!UICONTROL Delivered] | Loggas varje gång ett e-postmeddelande accepteras av mottagarens e-postserver. Detta innebär inte att skräppostfilter undviks. Det får bara finnas 1 leverans för varje skickat e-postmeddelande. |
| [!UICONTROL Hard Bounced] | Vissa studsar beror på skräppostblock, så vi försöker inte skicka den personen med e-post på 24 timmar i någon kampanj. Andra hårda studsar som icke-existerande inkorgar är permanenta och vi kommer aldrig att skicka ut personen igen från någon kampanj. |
| [!UICONTROL Soft Bounced] | Loggas när ett serversvar är oklart, postlådan är full eller allmänt förekommande serverproblem. Vi har verkligen gett dessa personer en återförsökslogik i 24-36 timmar för framtida leverans. Detta diskvalificerar inte personen från andra utskick. |
| [!UICONTROL Opened] | Loggas när en mottagare visar ett e-postmeddelande med bilder som INTE är blockerade. Endast en öppen händelse per e-post, per person, per smart kampanj loggas. Om de öppnar samma e-postmeddelande från sin inkorg två gånger loggas det inte mer än en gång. |
| [!UICONTROL Clicked] | Loggas varje gång en dekorerad URL från e-postmeddelandet läses in i webbläsaren (resultatet av att du klickade på länken). Vanligtvis är det här mottagaren som klickar, men det kan också vara en klipp ut/klistra in. |
| [!UICONTROL Unsubscribed] | Loggas när en person klickar på länken för att avbryta prenumerationen i ett e-postmeddelande och skickar in formuläret för att avbryta prenumerationen. |

>[!CAUTION]
>
>Om samma e-post skickas till samma person två gånger från samma kampanj loggas händelsen **[!UICONTROL Opened]** högst en gång.
