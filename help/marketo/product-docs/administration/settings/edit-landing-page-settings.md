---
unique-page-id: 2359918
description: Redigera inställningar för landningssida - Marketo Docs - produktdokumentation
title: Redigera inställningar för landningssida
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Redigera inställningar för landningssida {#edit-landing-page-settings}

Du kan redigera ditt domännamn och din reservsida, aktivera eller inaktivera förifyllning av formulär, förhindra missbruk av din landningssida och mycket annat. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Under **Administratör**, klicka **Landningssidor**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. I **Landningssidor** avsnitt, klicka **Redigera**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Ange domän- och sidinformation.

   | Villkor | Definition |
   |---|---|
   | Domännamn för landningssidor | Det här är din CNAME. En CNAME är den första delen av den URL som du ger personer för landningssidor. I `https://go.yourCompany.com`, ordet&quot;go&quot; är CNAME. Du kan ha flera, men de flesta använder bara den. |
   | Reservsida | Det är här du ska gå om landningssidan inte finns eller är nere. Läs mer om [reservsidor](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Hemsida | Ange företagets webbplats-URL. |

   ![](assets/three.png)

1. Kontrollera **Formulärförifyllning** kryssrutan för att tillåta formulär att förifylla information för kända (cookifyllda) personer. Avmarkera för att blockera.

   ![](assets/four.png)

1. Om du vill förhindra att en skadlig webbplats verkar vara värd för ditt innehåll ska du kontrollera **Tillåt inte att Marketo-sidor bäddas in på externa webbsidor** kryssrutan.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Om du vill ha förifyllningen `<script>` -tagg som ska visas i slutet av `<head>` -taggen i koden kontrollerar du **Injicera förifyllningsskript i slutet av huvudet** box. Låt alternativet vara avmarkerat om du vill att det ska visas i början.
   >
   >Kontrollera **Ta bort standardfavoritikonlänkar** för att förhindra att Marketo infogar några favoritikonlänkar i koden.

1. När du har gjort dina val klickar du på **Spara.**

   ![](assets/six.png)

   Bra jobbat! Dina landningssidor har nu rätt information och bör börja fungera direkt.
