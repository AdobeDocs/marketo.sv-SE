---
unique-page-id: 2359918
description: Redigera inställningar för landningssida - Marketo Docs - produktdokumentation
title: Redigera inställningar för landningssida
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Redigera inställningar för landningssida {#edit-landing-page-settings}

Du kan redigera ditt domännamn och din reservsida, aktivera eller inaktivera förifyllning av formulär, förhindra missbruk av din landningssida och mycket annat. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Administratör** område.

   ![](assets/edit-landing-page-settings-1.png)

1. Klicka **Landningssidor**.

   ![](assets/edit-landing-page-settings-2.png)

1. I **Landningssidor** avsnitt, klicka **Redigera**.

   ![](assets/edit-landing-page-settings-3.png)

1. Ange domän- och sidinformation.

   ![](assets/edit-landing-page-settings-4.png)

   | Villkor | Definition |
   |---|---|
   | Domännamn för landningssidor | Det här är din CNAME. En CNAME är den första delen av den URL som du ger personer för landningssidor. I `https://go.yourCompany.com`, ordet&quot;go&quot; är CNAME. Du kan ha flera, men de flesta använder bara den. |
   | Reservsida | Det är här du ska gå om landningssidan inte finns eller är nere. Läs mer om [reservsidor](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Hemsida | Ange företagets webbplats-URL. |

1. Kontrollera **Formulärförifyllning** kryssrutan för att tillåta formulär att förifylla information för kända (cookifyllda) personer. Avmarkera för att blockera.

   ![](assets/edit-landing-page-settings-5.png)

1. Om du vill förhindra att en skadlig webbplats verkar vara värd för ditt innehåll ska du kontrollera **Tillåt inte att Marketo-sidor bäddas in på externa webbsidor** kryssrutan.

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >Om du vill ha förifyllningen `<script>` -tagg som ska visas i slutet av `<head>` -taggen i koden kontrollerar du **Injicera förifyllningsskript i slutet av huvudet** box. Låt alternativet vara avmarkerat om du vill att det ska visas i början.
   >
   >Kontrollera **Ta bort standardfavoritikonlänkar** för att förhindra att Marketo infogar några favoritikonlänkar i koden.

1. När du har gjort dina val klickar du på **Spara.**

   ![](assets/edit-landing-page-settings-7.png)

   Bra jobbat! Dina landningssidor har nu rätt information och bör börja fungera direkt.
