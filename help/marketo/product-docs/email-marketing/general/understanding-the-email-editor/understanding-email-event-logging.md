---
unique-page-id: 1147356
description: Understanding Email Event Logging - Marketo Docs - produktdokumentation
title: E-posthändelseloggning
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Om e-posthändelseloggning {#understanding-email-event-logging}

När du skickar e-postmeddelanden loggar Marketo olika datapunkter till personens aktivitetsloggar. Här är de grundläggande.

| Händelse | Beskrivning |
|---|---|
| Skickat | Loggas varje gång ett e-postmeddelande skickas från Marketo-servrar, oavsett om det faktiskt levereras. Studsade e-postmeddelanden loggas fortfarande som&quot;Skickat&quot;. |
| Levererat | Loggas varje gång ett e-postmeddelande accepteras av mottagarens e-postserver. Detta innebär inte att skräppostfilter undviks. Det får bara finnas 1 leverans för varje skickat e-postmeddelande. |
| Hård studsad | Vissa studsar beror på skräppostblock, så vi försöker inte skicka den personen med e-post på 24 timmar i någon kampanj. Andra hårda studsar som icke-existerande inkorgar är permanenta och vi kommer aldrig att skicka ut personen igen från någon kampanj. |
| Mjuk studsad | Loggas när ett serversvar är oklart, postlådan är full eller allmänt förekommande serverproblem. Vi har verkligen gett dessa personer en återförsökslogik i 24-36 timmar för framtida leverans. Detta diskvalificerar inte personen från andra utskick. |
| Öppnad | Loggas när en mottagare visar ett e-postmeddelande med bilder som INTE är blockerade. Endast en öppen händelse per e-post, per person, per smart kampanj loggas. Om de öppnar samma e-postmeddelande från sin inkorg två gånger loggas det inte mer än en gång. |
| Klickat | Loggas varje gång en dekorerad URL från e-postmeddelandet läses in i webbläsaren (resultatet av att du klickade på länken). Vanligtvis är det här mottagaren som klickar, men det kan också vara en klipp ut/klistra in. |
| Avbeställ | Loggas när en person klickar på länken för att avbryta prenumerationen i ett e-postmeddelande och skickar in formuläret för att avbryta prenumerationen. |

>[!CAUTION]
>
>Om samma e-post skickas till samma person två gånger från samma kampanj loggas händelsen **Öppnad** högst en gång.
