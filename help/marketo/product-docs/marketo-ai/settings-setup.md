---
description: Lär dig hur du aktiverar Marketo AI-behörigheter, konfigurerar organisationsregler och hanterar inställningar som integreringar och meddelanden.
title: Inställningar och inställningar
beta: true
hide: true
hidefromtoc: true
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: 562442b6340d08aef492d4b3576c0d6b5f3d720d
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Inställningar och inställningar {#settings-setup}

Lär dig hur du aktiverar behörigheter och använder området Inställningar för att visa anslutningsinformation, definiera organisationsregler och konfigurera integreringar och meddelanden.

>[!NOTE]
>
>Den här funktionen är i en öppen betaversion och är för närvarande i en fasad lansering under de kommande månaderna. Du kommer att få veta när det har aktiverats för din prenumeration när du ser en _Build with AI_-platta på din Min Marketo-skärm.

## Behörigheter och roller {#permission-and-role}

Det finns en _Access Build med AI_-behörighet och en _Build med AI-användare_-roll, vilket ger administratörerna större kontroll över vilka användare som kan komma åt funktionen **Bygg med AI**. Behörigheten tilldelas på rollnivån. Rollen _Bygg med AI-användare_ har behörigheten _Åtkomstbygge med AI_ aktiverad som standard.

>[!IMPORTANT]
>
>_Åtkomstbygget med AI_-behörighet är inte aktiverat som standard för alla roller. Se tabellen nedan för mer information.

| Roll | Standardstatus |
| --- | --- |
| Administratör | Aktiverad |
| Adobe produktadministratör | Aktiverad |
| Marknadsförare | Handikappade |
| Standardanvändare | Inte tillgängligt |
| Skapa med AI-användare | Aktiverad |
| Anpassade roller | Handikappade |

### Åtkomstbygge med AI-behörighet {#access-build-with-ai-permission}

Följ stegen nedan för att aktivera _Access Build med AI_ för kvalificerade roller som inte redan har det aktiverat.

1. I My Marketo klickar du på **Admin** och sedan på **Användare och roller**.

   ![](assets/settings-setup-1.png)

1. Välj önskad roll på fliken _Roller_ och klicka på **Redigera roll**.

   ![](assets/settings-setup-2.png)

1. Bläddra nedåt och markera kryssrutan _Åtkomstbygge med AI_ och klicka på **Spara**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Du kan använda samma steg för att ta bort behörigheten genom att **un** markera kryssrutan _Access Build with AI_ .

### Bygg med AI-användarroll {#build-with-ai-user-role}

Följ de här stegen för att tilldela en specifik användare till rollen _Skapa med AI-användare_.

>[!NOTE]
>
>Den här rollen **endast** innehåller _Åtkomstbygge med AI_-behörighet.

1. I My Marketo klickar du på **Admin** och sedan på **Användare och roller**.

   ![](assets/settings-setup-1.png)

1. Markera önskad användare och klicka på **Redigera användare**.

   ![](assets/settings-setup-5b.png)

1. Markera kryssrutan _Skapa med AI-användare_ i _Roller och arbetsytor_. Om du har fler än en arbetsyta kan du ange vilka som ska få åtkomst i den nedrullningsbara signaturmenyn **+**. Klicka på **Spara** när du är klar.

   ![](assets/settings-setup-6b.png)

### Anpassad roll {#custom-role}

Du kan också [skapa en ny roll](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} och anpassa dess behörigheter, lägga till _Access Build med AI_, tillsammans med allt annat du vill ha, och [tilldela den rollen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} till specifika användare.

## Inställningar {#settings}

1. Klicka på rutan **Bygg med AI** i My Marketo.

   ![](assets/settings-setup-4.png)

1. Klicka på kugghjulet.

   ![](assets/settings-setup-5.png)

### Anslutning {#connection}

Fliken innehåller inte redigerbara fält. Här visas kontoinformation som ditt Munchkin ID och IMS-företag.

![](assets/settings-setup-6.png)

### Organisationsregler {#organizational-rules}

Definiera riktlinjer och begränsningar för organisationen som Marketo AI följer när du skapar eller ändrar Marketo Engage-resurser.

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Regler använder Markdown-format med YAML-förhandsgranskning. Globala regler gäller för alla arbetsytor. Workspace-regler åsidosätter globala inställningar.

### Integreringar (kommer snart) {#integrations}

Konfigurera anslutningar till externa tjänster och API:er.

_Den här fliken kan visas i användargränssnittet, men kan ännu inte användas. Kom tillbaka för uppdateringar_.

### Meddelanden (kommer snart) {#notifications}

Hantera aviseringsinställningar och meddelandekanaler.

_Den här fliken kan visas i användargränssnittet, men kan ännu inte användas. Kom tillbaka för uppdateringar_.
