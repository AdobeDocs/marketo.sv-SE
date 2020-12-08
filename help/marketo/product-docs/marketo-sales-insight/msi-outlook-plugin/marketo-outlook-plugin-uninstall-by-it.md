---
unique-page-id: 11382829
description: Marketo Outlook Plugin Uninstall by IT - Marketo Docs - Produktdokumentation
title: Marketo Outlook Plugin - avinstallation av IT
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Marketo Outlook Plugin - avinstallation av IT {#marketo-outlook-plugin-uninstall-by-it}

Så här kan IT-avdelningen fjärravinstallera Marketo Outlook-pluginprogrammet.

Kör följande kommandorad som System eller ett administratörskonto med växeln /x som ska avinstalleras.
`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exempel**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Vid felsökning kan du aktivera loggning för att skapa en utdataloggfil.  `<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exempel**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Om du vill ange en plats för loggfilerna kan du ange filsökvägen på kommandoraden.  `<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exempel**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Om du avinstallerar plugin-programmet från en fjärrdator stängs Outlook på användarens dator.

Se [Microsofts fullständiga lista över växlar](https://support.microsoft.com/en-us/kb/227091) om du vill prova olika loggningsnivåer eller användargränssnittsnivåer.