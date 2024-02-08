---
description: Skapa ett interaktivt webbinarium - Marketo Docs - produktdokumentation
title: Skapa ett interaktivt webbinarium
exl-id: 91fdede6-2e5a-4895-9893-852d0441aa2a
feature: Interactive Webinars
source-git-commit: 77300e8d620887b5c1d14a4f979a96488b6eec87
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Skapa ett interaktivt webbinarium {#create-an-interactive-webinar}

Skapa ett interaktivt webbinarium i några enkla steg.

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/create-an-interactive-webinar-1.png)

1. Högerklicka på önskad mapp och välj **Nytt program**.

   ![](assets/create-an-interactive-webinar-2.png)

1. Ge programmet ett namn. Under Programtyp väljer du **Händelse**.

   ![](assets/create-an-interactive-webinar-3.png)

1. Klicka på listrutan Kanal och välj en kanal som har _Händelse med webbinarium_ i kolumnen&quot;Tillämpar på&quot;. I det här exemplet väljer vi **Webbinarium**.

   ![](assets/create-an-interactive-webinar-4.png)

   >[!NOTE]
   >
   >För att se vilka kanaler som gäller _Händelse med webbinarium_, gå till **Administratör** > **Taggar**. &quot;Gäller för&quot; ska vara den mittersta kolumnen. Läs mer om Tillämpa på i steg 5 i [den här artikeln](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.

1. Välj **Interaktiva webbinarier** och klicka **Nästa**.

   ![](assets/create-an-interactive-webinar-5.png)

   >[!NOTE]
   >
   >Information om partnerwebbinarier finns här.

1. Ange maximal målgruppsstorlek för webbinariet och hur länge det ska vara.

   ![](assets/create-an-interactive-webinar-6.png)

1. Schemalägg datum/tid för webbinariet och klicka på **Skapa**.

   ![](assets/create-an-interactive-webinar-7.png)

Ditt interaktiva webbinarium skapas. Nu kan du lägga till ett webbinarium.

## Webinar Team {#webinar-team}

Ett webbinarium i Interactive Webinars består av alla roller som bidrar till att det webbinarium som finns i Adobe Connect kan levereras utan problem. Detta omfattar både presentatörer och andra.

>[!NOTE]
>
>Presentatörer och medvärdar i Marketo mappar exakt till presentatörens och medarbetarnas roller under webbseminariet i Adobe Connect.

Presentatören är en extern roll som deltar i framtagningen av webbinariet, medan andra kan vara presentatörer och hantera administrativa aspekter av webbseminariedistributionen. Medvärdarna kan vara både interna och externa. Externa värdar har inte tillgång till Interactive Webinar Event Programs i Marketo, men har medvärdbehörighet under leverans i Adobe Connect. Interna värdar får tillgång till både Interactive Webinar Event Program i Marketo och får även medvärdbehörighet under leveransen. Detta säkerställer att de interna värdarna kan ta del av Interactive Webinars Event Program när den som skapade det interaktiva webbinariet inte längre är med i Interactive Webinars användaruppsättning, eller inte ens en Marketo-användare.

### Lägga till ett webbinarium {#adding-a-webinar-team}

Om du vill lägga till en medvärd eller presentatör klickar du på **Lägg till värdar** eller **Lägg till presentatörer** på skärmen Översikt.

![](assets/create-an-interactive-webinar-8.png)

Vid klickning **Lägg till presentatörer** uppmanas du att ange deras förnamn, efternamn och e-postadress. Denna information kommer att göras tillgänglig för Adobe Connect under leveransen av webbinariet så att rätt information kan fyllas i automatiskt utan att användaren behöver ange dem under bidraget för leverans via webbinariet. En sammanfogad URL fylls i för alla presentatörer och kan delas av den som skapat den.

Vid klickning **Lägg till värdar** blir du ombedd att lägga till antingen en intern eller extern användare. Om du väljer internal kan du välja önskad användare i listan över alla användare som har lagts till som interaktiva webbinarier i Marketo Engage. Om du väljer extern uppmanas du att lägga till förnamn, efternamn och e-post-ID (ungefär som när du lägger till en presentatör). Du kan också hämta kopplade URL:er för både interna och externa användare som ska delas med dem.

När du har lagt till ett webbinarium kan du klicka på kopieringsikonen bredvid varje användare för att kopiera (och sedan dela) deras kopplade URL:er.

<br>

Nu är det dags att [utforma ditt webbinarium](/help/marketo/product-docs/demand-generation/events/interactive-webinars/designing-interactive-webinars.md){target="_blank"}.
