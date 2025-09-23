---
description: Behörigheter - Marketo Docs - produktdokumentation
title: Behörigheter
feature: Dynamic Chat
exl-id: 06798ac4-636b-476e-bbb1-498062844406
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Behörigheter {#permissions}

Det finns fem standardprofiler med fördefinierade behörigheter som du kan redigera i Dynamic Chat. Du kan också skapa en anpassad profil med en anpassad uppsättning behörigheter. Vi går igenom båda.

## Redigera befintliga behörigheter {#edit-existing-permissions}

1. Klicka på [Dynamic Chat](https://adminconsole.adobe.com/){target="_blank"} i **Adobe Admin Console**.

   ![](assets/permissions-1.png)

1. Välj den profil som du vill redigera på fliken **Produktprofiler**. I det här exemplet väljer vi **Live Agent**.

   ![](assets/permissions-2.png)

1. Klicka på fliken **Behörigheter**.

   ![](assets/permissions-3.png)

1. Markera området i profilen som du vill redigera. I det här exemplet väljer vi Live Chat. Klicka på pennikonen.

   ![](assets/permissions-4.png)

1. Tillgängliga behörighetsobjekt visas till vänster. Du kan välja att lägga till behörigheter en i taget eller alla på en gång. Klicka på **+**-tecknet.

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >Om du aktiverar Inkludera automatiskt läggs alla behörighetsobjekt till i den inkluderade listan. När nya behörighetsobjekt blir tillgängliga inkluderas de automatiskt för den produktprofilen.

1. Klicka på **Spara**.

   ![](assets/permissions-6.png)

Nu kan du upprepa den här processen för alla andra Dynamic Chat-områden.

![](assets/permissions-7.png)

## Skapa en profil {#create-a-profile}

1. Klicka på [Dynamic Chat](https://adminconsole.adobe.com/){target="_blank"} i **Adobe Admin Console**.

   ![](assets/permissions-8.png)

1. Klicka på **Ny profil** på fliken **Produktprofiler**.

   ![](assets/permissions-9.png)

1. **Namn** din produktprofil. Du kan också ge den ett visningsnamn och/eller en beskrivning och välja att låta användare få meddelanden när de läggs till/tas bort. Klicka på **Spara** när du är klar.

   ![](assets/permissions-10.png)

1. Den nya profilen visas på fliken Produktprofiler. Markera den.

   ![](assets/permissions-11.png)

1. Följ nu steg 3-6 från [avsnittet ovan](#edit-existing-permissions) för varje önskat område.

## Lista över behörigheter {#list-of-permissions}

Här nedan finns en lista med alla tillgängliga behörigheter för varje område.

<table>
<thead>
  <tr>
    <th style="width:25%">Dynamic Chat Area</th>
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
    <td><li>Visa mina konversationer</li>
    <li>Visa alla konversationer</li>
  </tr>
  <tr>
    <td>Möten</td>
    <td><li>Hantera alla möten</li>
  </tr>
  <tr>
    <td>Analytics </td>
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
    <td><li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Hantera anpassade regler (lägg till, redigera, ta bort)</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Hantera konton (lägg till, redigera, ta bort) <b>*</b></li>
    <li>Hantera Chatbot-inställningar</li>
    <li>Hantera inställningar för konversationsflöden</li>
    <li>Hantera integritet och säkerhet</li>
    <li>Hantera integreringar</li>
    <li>Hantera agenter</li>
    <li>Visa agentteam <b>*</b></li>
    <li>Hantera agentteam (lägg till, redigera, ta bort) <b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;** är för närvarande endast tillgängligt för användare av Dynamic Prime

<p>

## Standardprofilbehörigheter {#default-profile-permissions}

Nedan visas de fem standardprofilerna och de behörigheter som är aktiverade som standard.

<table>
<thead>
  <tr>
    <th style="width:25%">Profil</th>
    <th>Standardbehörigheter</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Marknadsförare</td>
    <td><i>Konversationshantering</i>
    <li>Visa dialogrutor</li>
    <li>Hantera dialogrutor (skapa, ta bort)</li>
    <li>Publicera dialogrutor</li>
    <li>Visa konversationsflöden</li>
    <li>Hantera konversationsflöden (skapa, ta bort)</li>
    <li>Publicera konversationsflöden</li>
    <br>
    <i> Live-chatt </i>
    <li>n/a</li>
    <br>
    <i>Möten</i>
    <li>n/a</li>
    <br>
    <i> Analyser </i>
    <li>Visa globala prestandarapporter</li>
    <li>Visa chattrapporter live</li>
    <li>Visa mötesrapporter</li>
    <br>
    <i> Agentinställningar </i>
    <li>n/a</li>
    <br>
    <i> Administratörsinställningar </i>
    <li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Visa agentteam <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Live Agent</b></td>
    <td><i>Konversationshantering</i>
    <li>Visa dialogrutor</li>
    <li>Visa konversationsflöden</li>
    <br>
    <i> Live-chatt </i>
    <li>Visa mina konversationer</li>
    <br>
    <i>Möten</i>
    <li>n/a</li>
    <br>
    <i> Analyser </i>
    <li>Visa globala prestandarapporter</li>
    <li>Visa chattrapporter live</li>
    <li>Visa mötesrapporter</li>
    <br>
    <i> Agentinställningar </i>
    <li>Hantera chatttillgänglighet live</li>
    <li>Anslut din kalender</li>
    <li>Hantera kalendertillgänglighet</li>
    <br>
    <i> Administratörsinställningar </i>
    <li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Visa agentteam <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Kalenderagent</b></td>
    <td><i>Konversationshantering</i>
    <li>Visa dialogrutor</li>
    <li>Visa konversationsflöden</li>
    <br>
    <i> Live-chatt </i>
    <li>n/a</li>
    <br>
    <i>Möten</i>
    <li>n/a</li>
    <br>
    <i> Analyser </i>
    <li>Visa globala prestandarapporter</li>
    <li>Visa chattrapporter live</li>
    <li>Visa mötesrapporter</li>
    <br>
    <i> Agentinställningar </i>
    <li>Anslut din kalender</li>
    <li>Hantera kalendertillgänglighet</li>
    <br>
    <i> Administratörsinställningar </i>
    <li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Visa agentteam <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Marknadsföringsadministratör</b></td>
    <td><i>Konversationshantering</i>
    <li>Visa dialogrutor</li>
    <li>Hantera dialogrutor (skapa, ta bort)</li>
    <li>Publicera dialogrutor</li>
    <li>Visa konversationsflöden</li>
    <li>Hantera konversationsflöden (skapa, ta bort)</li>
    <li>Publicera konversationsflöden</li>
    <br>
    <i> Live-chatt </i>
    <li>n/a</li>
    <br>
    <i>Möten</i>
    <li>n/a</li>
    <br>
    <i> Analyser </i>
    <li>Visa globala prestandarapporter</li>
    <li>Visa chattrapporter live</li>
    <li>Visa mötesrapporter</li>
    <li>Exportera rapporter</li>
    <br>
    <i> Agentinställningar </i>
    <li>n/a</li>
    <br>
    <i> Administratörsinställningar </i>
    <li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Hantera anpassade regler (lägg till, redigera, ta bort)</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Hantera konton (lägg till, redigera, ta bort) <b>*</b></li>
    <li>Hantera Chatbot-inställningar</li>
    <li>Hantera inställningar för konversationsflöden</li>
    <li>Hantera integritet och säkerhet</li>
    <li>Hantera integreringar</li>
    <li>Visa agentteam <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Försäljningsadministratör</b></td>
    <td><i>Konversationshantering</i>
    <li>Visa dialogrutor</li>
    <li>Visa konversationsflöden</li>
    <br>
    <i> Live-chatt </i>
    <li>Visa mina konversationer</li>
    <li>Visa alla konversationer</li>
    <br>
    <i>Möten</i>
    <li>Hantera alla möten</li>
    <br>
    <i> Analyser </i>
    <li>Visa globala prestandarapporter</li>
    <li>Visa chattrapporter live</li>
    <li>Visa mötesrapporter</li>
    <li>Exportera rapporter</li>
    <br>
    <i> Agentinställningar </i>
    <li>Hantera chatttillgänglighet live</li>
    <li>Anslut din kalender</li>
    <li>Hantera kalendertillgänglighet</li>
    <br>
    <i> Administratörsinställningar </i>
    <li>Visa Round-robin</li>
    <li>Visa anpassade regler</li>
    <li>Hantera anpassade regler (lägg till, redigera, ta bort)</li>
    <li>Visa kontolista <b>*</b></li>
    <li>Hantera konton (lägg till, redigera, ta bort) <b>*</b></li>
    <li>Hantera agenter</li>
    <li>Visa agentteam <b>*</b></li>
    <li>Hantera agentteam <b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;** är för närvarande endast tillgängligt för användare av Dynamic Prime
