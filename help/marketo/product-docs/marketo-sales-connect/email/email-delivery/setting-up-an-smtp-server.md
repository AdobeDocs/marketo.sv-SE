---
unique-page-id: 14746594
description: Konfigurera en SMTP-server - Marketo Docs - Produktdokumentation
title: Konfigurera en SMTP-server
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---


# Konfigurera en SMTP-server {#setting-up-an-smtp-server}

## Översikt {#overview}

**Vad är en SMTP-server?**

**** Simple **** Mail **** Transfer **** Protocol, det här är servern som ansvarar för att skicka utgående e-post. När du skickar ett e-postmeddelande från din e-postklient använder du samma tjänst för att leverera e-postmeddelandet.

**Varför vill jag konfigurera min SMTP-server med Sales Connect?**

Det gör att ni kan utnyttja företagets anseende och leveransförmåga och inte behöver förlita er på andras. Våra standardservrar för MSC ingår i en delad IP-pool, vilket innebär att de skickas från ett delat rykte. Vi rekommenderar att ditt team skapar en egen leveranskanal med Sales Connect.

**Hur skickar Sales Connect till min SMTP-server?**

Följ [de här stegen](http://docs.marketo.com/x/ZgPh).

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **Behöver jag konfigurera något i min e-postklient?**

När det gäller en leveranskanal, nej. När du har installerat tillägget använder Sales Connect samma leveranskanal som du konfigurerade för att skicka e-post.

## Hämta SMTP-autentiseringsuppgifter {#getting-the-smtp-credentials}

**Hur får jag mina SMTP-inloggningsuppgifter?**

Kontakta IT-avdelningen för att ta reda på vilken leveranskanal ert företag använder för att skicka e-post och hur ni får tillgång till era SMTP-uppgifter. Beroende på hur servern är konfigurerad kan det finnas anpassade värden för SMTP-servernamnet eller serverporten. Om du inte har något dedikerat IT-team kan du kontakta din e-postleverantör.

**Vad har jag för alternativ om mitt företag använder Office365?**

Proffs

* Lätt att installera
* Alla användare med ett Office365-konto har åtkomst till den här SMTP-servern

Kon

* Begränsning kan förekomma
* Varje användare måste själv konfigurera detta
* Om du ändrar användarens O365-lösenord bryts anslutningen

Om du använder Office365 eller Exchange Online kan du ansluta till SMTP-servern med hjälp av en standarduppsättning med autentiseringsuppgifter. Kom ihåg att Office365 inte är en massutskick av e-post, men det fungerar bra för att skicka engångskommunikation via e-post. När du skickar massutskick kan Office365 begränsa dina e-postmeddelanden, vilket kan leda till felaktig leverans. Läs mer om den här artikeln från Microsoft om [hur du konfigurerar SMTP-klientinlämning](http://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4).
`<blockquote>  <p>“You can only send from one email address unless your device can store login credentials for multiple Office 365 mailboxes. Office 365 imposes a limit of 30 messages sent per minute, and a limit of 10,000 recipients per day.”</p> </blockquote>`\
Om du bestämmer dig för att använda Office365 som leveranskanal måste du ange dessa autentiseringsuppgifter. Samma inloggningsuppgifter kan inte användas i hela teamet eftersom Office365 använder användarens e-postadress och lösenord för att ansluta.

Microsoft och massutskick

[Klicka här](http://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) om du vill veta mer om massutskick i Office365.
`<blockquote>  <p>“Exchange Online customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.”</p> </blockquote>`\
**Vad händer om mitt företag använder Gmail?**

Du behöver inte hämta några SMTP-autentiseringsuppgifter om ditt team vill använda Gmail som leveranskanal med Sales Connect. Med Sales Connect får användarna tillgång till sin Gmail-leveranskanal via vår OAuth-integrering. Användarna kan aktivera detta genom att integrera sitt Sales Connect-konto med Gmail.

![](assets/2.png)

**Kan jag dela samma SMTP-inloggningsuppgifter med hela mitt team?**

Detta beror på vilken leveranskanal du använder. Till exempel tillåter tjänster som Sparkpost att autentiseringsuppgifterna är domänbaserade, så att alla som skickar med en viss domän autentiseras för att skicka via den servern. Om så är fallet, ja, kan du dela autentiseringsuppgifterna med teamet.

Om du ansluter till Office365 är autentiseringsuppgifterna e-postadressbaserade. Detta innebär endast den e-postadress som upprättade anslutningen autentiseras för att skicka e-post via den leveranskanalen, så autentiseringsuppgifterna bör **inte** delas.

![](assets/3.png)

