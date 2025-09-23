---
unique-page-id: 11382815
description: Marketo [!DNL Outlook] Plugin-installation av IT - Marketo Docs - Produktdokumentation
title: Marketo [!DNL Outlook] Plugin-installation av IT
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Marketo [!DNL Outlook] - Plugin-installation av IT {#marketo-outlook-plugin-installation-by-it}

Ibland kräver företagets policyer att IT-teamet installerar all programvara på sina medarbetares datorer. I sådana fall gör IT-avdelningen ofta detta via fjärranslutning med sin egen programvara. Det här dokumentet innehåller de kommandorader som du skulle använda som indata under distributionsprocessen för att fjärrinstallera plugin-programmet för Outlook.

>[!PREREQUISITES]
>
>[Konfigurera ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) företagsnyckeln.

Kör följande kommandorad som System eller ett administratörskonto med växeln /i som ska installeras.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exempel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

För felsökning kan du aktivera loggning för att skapa en utdataloggfil.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exempel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Om du vill ange en plats för loggfilerna kan du ange filsökvägen på kommandoraden.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exempel**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Loggfilens lagringsplats måste finnas, annars avbryts installationen.

Se [Microsoft fullständiga lista över växlar](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) om du vill prova olika loggningsnivåer eller användargränssnittsnivåer.

>[!MORELIKETHIS]
>
>[Marketo [!DNL Outlook] Avinstallera plugin-program av IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
