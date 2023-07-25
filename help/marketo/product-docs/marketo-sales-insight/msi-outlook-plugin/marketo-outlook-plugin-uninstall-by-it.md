---
unique-page-id: 11382829
description: Marketo Outlook Plugin Uninstall by IT - Marketo Docs - Produktdokumentation
title: Avinstallera Marketo Outlook-plugin med IT
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# Avinstallera Marketo Outlook-plugin med IT {#marketo-outlook-plugin-uninstall-by-it}

Så här kan IT-avdelningen fjärravinstallera Marketo Outlook-pluginprogrammet.

Kör följande kommandorad som System eller ett administratörskonto med växeln /x som ska avinstalleras.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exempel**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Vid felsökning kan du aktivera loggning för att skapa en utdataloggfil.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exempel**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Om du vill ange en plats för loggfilerna kan du ange filsökvägen på kommandoraden.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exempel**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Om du avinstallerar plugin-programmet från en fjärrdator stängs Outlook på användarens dator.

Se [Microsoft kompletta lista över switchar](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) om du vill prova olika loggningsnivåer eller användargränssnittsnivåer.
