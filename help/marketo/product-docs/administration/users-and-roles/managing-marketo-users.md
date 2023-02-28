---
unique-page-id: 2359906
description: Hantera Marketo-användare - Marketo Docs - produktdokumentation
title: Hantera Marketo-användare
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
source-git-commit: 3bb7e8155491f810cc0e71637482e6da788dc068
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Hantera Marketo-användare {#managing-marketo-users}

## Skapa användare {#create-users}

1. Gå till **Administratör** område.

   ![](assets/managing-marketo-users-1.png)

1. Klicka **Användare och roller**.

   ![](assets/managing-marketo-users-2.png)

1. Klicka **Bjud in ny användare**.

   ![](assets/managing-marketo-users-3.png)

1. Ange **E-postadress**, **Förnamn** och **Efternamn**.

   ![](assets/managing-marketo-users-4.png)

1. Du kan också ange en orsak till inbjudan och välja ett förfallodatum i dialogrutan **Åtkomst upphör** med datumväljaren.

   ![](assets/managing-marketo-users-5.png)

1. Klicka **Nästa**.

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >Ett förfallodatum passar bra för kortsiktiga externa intressenter eller konsulter som bara behöver tillgång till Marketo under en kort tid.

   >[!NOTE]
   >
   >När förfallodatumet inkommer får användaren ett meddelande om förfallodatum och kontot är låst.

1. Välj **Roll** efter eget val och klicka **Nästa**.

   ![](assets/managing-marketo-users-7.png)

1. Redigera inbjudningsmeddelandet om det behövs. Klicka **Skicka**.

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >E-postadressen/inloggningen måste vara unik; om du redan har använt den i en sandlådeinstans måste du använda en annan i produktionen och vice versa.

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >Inbjudningarna går ut tre dagar efter att en ny användare har lagts till.

Den nya användaren visas nu på fliken Användare och får ett e-postmeddelande med instruktioner om hur du aktiverar kontot.

## Ta bort användare {#delete-users}

1. Gå till **Administratör** område.

   ![](assets/managing-marketo-users-10.png)

1. Klicka **Användare och roller**.

   ![](assets/managing-marketo-users-11.png)

1. Markera den användare som du vill ta bort och klicka på **Ta bort användare**.

   ![](assets/managing-marketo-users-12.png)

1. Bekräfta genom att klicka **OK**.

   ![](assets/managing-marketo-users-13.png)

## Återställ användarlösenord {#reset-user-passwords}

1. Gå till området Admin.

   ![](assets/managing-marketo-users-14.png)

1. Klicka **Användare och roller**.

   ![](assets/managing-marketo-users-15.png)

1. Välj en användare och klicka på **Återställ lösenord**.

   ![](assets/managing-marketo-users-16.png)

1. Klicka **Stäng** för att stänga uppmaningen.

   ![](assets/managing-marketo-users-17.png)

Användaren får ett e-postmeddelande med instruktioner för lösenordsåterställning.

>[!TIP]
>
>Om användaren inte ser e-postmeddelandet i sin inkorg ber du dem att kontrollera skräppostmappen.

## Ändra behörigheter och redigera användarinformation {#change-permissions-and-edit-user-information}

1. Gå till **Administratör** område.

   ![](assets/managing-marketo-users-18.png)

1. Klicka **Användare och roller**.

   ![](assets/managing-marketo-users-19.png)

1. Välj en användare och klicka på **Redigera användare**.

   ![](assets/managing-marketo-users-20.png)

1. Du kan redigera användarinformation och ändra den associerade rollen. Klicka **Spara**.

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>Om du är den enda administratören i Marketo ska du inte ta bort dina egna administratörsrättigheter.

>[!NOTE]
>
>Om en ny användare är inbjuden som administratör, eller om en administratör tas bort, får alla aktuella administratörer ett e-postmeddelande.

Fantastiskt arbete! Nu vet du hur du skapar en användare, tar bort en användare, återställer användarens lösenord och redigerar användare.
