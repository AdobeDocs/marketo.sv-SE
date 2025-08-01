---
unique-page-id: 11382829
description: Marketo [!DNL Outlook] Plugin Uninstall by IT - Marketo Docs - Produktdokumentation
title: Marketo [!DNL Outlook] Plugin-avinstallation av IT
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Marketo [!DNL Outlook] Plugin Uninstall av IT {#marketo-outlook-plugin-uninstall-by-it}

Så här kan IT-avdelningen fjärravinstallera Marketo [!DNL Outlook]-pluginprogrammet.

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
>Om du avinstallerar plugin-programmet på fjärrbasis stängs [!DNL Outlook] av på användarens dator.

Se [Microsoft fullständiga lista över växlar](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) om du vill testa olika loggningsnivåer eller användargränssnittsnivåer.
