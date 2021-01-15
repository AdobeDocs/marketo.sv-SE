---
unique-page-id: 2359918
description: Redigera inställningar för landningssida - Marketo Docs - Produktdokumentation
title: Redigera inställningar för landningssida
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Redigera inställningar för landningssida {#edit-landing-page-settings}

Du kan redigera ditt domännamn och din reservsida, aktivera eller inaktivera förifyllning av formulär, förhindra missbruk av din landningssida och mycket annat. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Under **Admin** klickar du på **Startsidor**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Klicka på **Redigera** i avsnittet **Startsidor**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Ange domän- och sidinformation.

   | Villkor | Definition |
   |---|---|
   | Domännamn för landningssidor | Det här är din CNAME. En CNAME är den första delen av den URL som du ger personer för landningssidor. I `http://go.yourCompany.com` är till exempel ordet &quot;go&quot; CNAME. Du kan ha flera, men de flesta använder bara den. |
   | Reservsida | Det är här du ska gå om landningssidan inte finns eller är nere. Läs mer om [reservsidor](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Hemsida | Ange företagets webbplats-URL. |

   ![](assets/three.png)

1. Markera kryssrutan **Förifyll formulär** om du vill att formulär ska kunna förifylla information för kända (cookies) personer. Avmarkera för att blockera.

   ![](assets/four.png)

1. Om du vill förhindra att en skadlig webbplats verkar vara värd för ditt innehåll markerar du kryssrutan **Tillåt inte att Marketo-sidor bäddas in i externa webbsidor**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Om du vill att förifyllningstaggen `<script>` ska visas i slutet av taggen `<head>` i koden markerar du rutan **Inmatningsskript i slutet av HEAD**. Låt alternativet vara avmarkerat om du vill att det ska visas i början.
   >
   >Markera **Ta bort standardfavoritikonlänkar** om du inte vill att Marketo ska infoga favoritikonlänkar i koden.

1. När du har gjort dina val klickar du på **Spara.**

   ![](assets/six.png)

   Bra jobbat! Dina landningssidor har nu rätt information och bör börja fungera direkt.
