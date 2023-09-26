---
description: Behörigheter - Marketo Docs - produktdokumentation
title: Behörigheter
feature: Dynamic Chat
source-git-commit: d60b506f0c84fc2883054be628817374d3a1a09b
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Behörigheter {#permissions}

Det finns fem standardprofiler med fördefinierade behörigheter som du kan redigera i Dynamic Chat. Du kan också skapa en anpassad profil med en anpassad uppsättning behörigheter. Vi går igenom båda.

## Redigera befintliga behörigheter {#edit-existing-permissions}

1. I [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, klicka **Dynamic Chat**.

   ![](assets/permissions-1.png)

1. I **Produktprofiler** markerar du den profil som du vill redigera. I det här exemplet väljer vi **Live Agent**.

   ![](assets/permissions-2.png)

1. Klicka på **Behörigheter** -fliken.

   ![](assets/permissions-3.png)

1. Markera området i profilen som du vill redigera. I det här exemplet väljer vi Live Chat. Klicka på pennikonen.

   ![](assets/permissions-4.png)

1. Tillgängliga behörighetsobjekt visas till vänster. Du kan välja att lägga till behörigheter en i taget eller alla på en gång. I det här exemplet finns det bara en tillgänglig, så vi lägger till den. Klicka på **+** signera.

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >Om du aktiverar Inkludera automatiskt läggs alla behörighetsobjekt till i den inkluderade listan. När nya behörighetsobjekt blir tillgängliga inkluderas de automatiskt för den produktprofilen.

1. Klicka **Spara**.

   ![](assets/permissions-6.png)

Nu kan du upprepa den här processen för alla andra Dynamic Chat-områden.

![](assets/permissions-7.png)

## Skapa en profil {#create-a-profile}

1. I [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, klicka **Dynamic Chat**.

   ![](assets/permissions-8.png)

1. I **Produktprofiler** flik, klicka **Ny profil**.

   ![](assets/permissions-9.png)

1. **Namn** din produktprofil. Du kan också ge den ett visningsnamn och/eller en beskrivning och välja att låta användare få meddelanden när de läggs till/tas bort. Klicka **Spara** när det är klart.

   ![](assets/permissions-10.png)

1. Den nya profilen visas på fliken Produktprofiler. Markera den.

   ![](assets/permissions-11.png)

1. Följ nu steg 3-6 från [avsnitt ovan](#edit-existing-permissions) för varje önskat område.


## Lista över behörigheter {#list-of-permissions}

Här nedan finns en lista med alla tillgängliga behörigheter för varje område.

<table>
<thead>
  <tr>
    <th style="width:30%">Dynamic Chat</th>
    <th>Behörigheter</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationshantering</td>
    <td><li>Visa dialogrutor</li>
    <li>Hantera dialogrutor (skapa, ta bort)</li>
    <li>Publicera dialogrutor</li>
    <li>Visa konversationsflöden</li>
    <li>Hantera konversationsflöden (skapa, ta bort)</li>
    <li>Publicera konversationsflöden</li></td>
  </tr>
  <tr>
    <td>Live Chatt</td>
    <td><li>Agent Inbox</li>
    <li>Visa mina konversationer</li>
    <li>Visa alla konversationer</li>
    <li>Visa konversationssammanfattning <b>*</b></li>
    <li>Visa assisterade svar <b>*</b></li></td>
  </tr>
  <tr>
    <td>Möten</td>
    <td><li>Hantera alla möten</li>
    <li>Hantera mina möten</li></td>
  </tr>
  <tr>
    <td>Analyser</td>
    <td><li>Visa globala prestandarapporter</li>
    <li>Visa chattrapporter live</li>
    <li>Visa mötesrapporter</li>
    <li>Exportera rapporter</li></td>
  </tr>
  <tr>
    <td>Agentinställningar</td>
    <td><li>Hantera chatttillgänglighet live</li>
    <li>Anslut din kalender</li>
    <li>Hantera kalendertillgänglighet</li></td>
  </tr>
  <tr>
    <td>Administratörsinställningar</td>
    <td><li>Visa arbetsytor <b>*</b></li>
    <li>Hantera arbetsytor (skapa, redigera, ta bort) <b>*</b></li>
    <li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Hantera anpassade regler (lägg till, redigera, ta bort)</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Hantera konton (lägg till, redigera, ta bort) <b>*</b></li>
    <li>Hantera Chatbot-inställningar</li>
    <li>Hantera inställningar för konversationsflöden</li>
    <li>Hantera integritet och säkerhet</li>
    <li>Hantera integreringar</li>
    <li>Hantera språk <b>*</b></li>
    <li>Hantera agenter</li>
    <li>Visa agentteam <b>*</b></li>
    <li>Hantera agentteam (lägg till, redigera, ta bort) <b>*</b></li>
    <li>Visa användningsgränser</li></td>
  </tr>
</tbody>
</table>

**&#42;** Endast tillgängligt för Dynamic Prime-användare
