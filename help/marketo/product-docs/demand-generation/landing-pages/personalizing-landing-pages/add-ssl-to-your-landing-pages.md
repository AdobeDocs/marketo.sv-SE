---
unique-page-id: 2359828
description: Lägg till SSL på era landningssidor - Marketo Docs - produktdokumentation
title: Lägg till SSL på era landningssidor
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: df7c5bfc344d5a22632128ef70b2c5c12d2f669d
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Lägg till SSL på era landningssidor {#add-ssl-to-your-landing-pages}

Med SSL-kryptering (Secure Socket Layer) kan du göra alla dina landningssidor för en Marketo Engage-instans säkra.

När du fyller i ett webbformulär eller besöker en landningssida som Marketo Engage är värd för, skickas informationen som standard via ett osäkert protokoll (HTTP). Enligt företagets policy kanske du vill skydda den information som skickas till Marketo via HTTPS. När du till exempel besöker `http://info.mydomain.com/` blir det nu `https://info.mydomain.com/`.

Marketo Engage spårar &quot;Besökt webbsida&quot; och &quot;Klicka på länk på webbsida&quot; som standard över osäkra HTTP-protokoll. Om du vill att dina spårningslänkar ska vara skyddade med deras egna certifikat måste du ha Marketo som en separat icke-delad server för att kunna aktivera den. För att skydda alla aspekter av en kontakts interaktion med dig måste du vanligtvis skydda både landningssidor och spårningslänkar.

## Aktivera SSL-certifiering {#enable-ssl-certification}

Lägg automatiskt till SSL för alla domänalias som du skapar som en del av reglerna för landningssidan.

1. Gå till området **Admin**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Välj **Landningssidor** i trädet. Klicka på listrutan **Nytt** på fliken **Regler** och välj **Nytt domänalias**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Ange ditt _domänalias_ och _standardsida_. Markera kryssrutan **Skapa SSL-certifikat**. Klicka på **Skapa** när du är klar.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Detta lägger automatiskt till ett SSL-certifikat för den här domänen.

## Aktivera SSL för din standarddomän {#enable-ssl-default-domain}

Följ stegen nedan för att aktivera SSL för din standarddomän.

1. I avsnittet **Admin** väljer du **Startsidor**. Klicka på den orangefärgade knappen **Redigera** bredvid _Inställningar_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Om du vill kan du även ändra domännamnet här (en giltig domän krävs).

1. Markera kryssrutan Generera SSL-certifikat och klicka på Spara.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* Kolumnen för SSL-certifikat i listan visar certifikatstatus för alla domänalias som skapats efter att den här funktionen släpptes (25 april 2025). Om SSL har aktiverats för en domän via Marketo Support finns certifikatet kvar, men visas inte i tabellen. Den här tabellen visar endast SSL-certifikat för domäner som lagts till med stegen i den här artikeln.
>
>* Det kan ta upp till tre minuter innan SSL är i READY-läge. Du måste uppdatera sidan för att ändringarna ska visas.

## Felmeddelanden {#error-messages}

Här nedan hittar du felmeddelanden som du kan få tillsammans med deras definitioner.

<table><thead>
  <tr>
    <th>Fel</th>
    <th>Information</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Ett oväntat fel uppstod när en domän skapades. Kontakta supporten om du behöver hjälp.</i></td>
    <td>Ett oväntat fel har inträffat. Hämta loggar och felinformation och eskalera problemet till <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo Support</a>.</td>
  </tr>
  <tr>
    <td><i>Det gick inte att hitta standarddomänen. Kontakta supporten om du behöver hjälp.</i></td>
    <td>Det uppstod ett problem när standarddomänen skulle hittas. Kontakta supporten så att de kan undersöka saken.</td>
  </tr>
  <tr>
    <td><i>SSL-certifikatet har redan utfärdats.</i></td>
    <td>Det finns redan ett SSL-certifikat för den här anpassade domänen. Ingen ytterligare åtgärd krävs såvida inte certifikatet har upphört att gälla eller behöver utfärdas på nytt.</td>
  </tr>
  <tr>
    <td><i>Domänen är inte mappad till standarddomänen.</i></td>
    <td>Den anpassade domänen är inte korrekt mappad till standarddomänen. Kontrollera inställningarna för domänmappning och se till att DNS-konfigurationen pekar på rätt standarddomän.</td>
  </tr>
  <tr>
    <td><i>Domänen finns redan.</i></td>
    <td>Det finns redan en domän med samma namn.</td>
  </tr>
</tbody></table>

## Saker att notera {#things-to-note}

* **DNS-mappning för domän till Marketo Engage**: Innan du lägger till domäner i användargränssnittet måste du [mappa CNAME:er till en domän som tillhandahålls av Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Anpassade SSL:er**: Om du behöver en anpassad SSL:er skickar du en [supportanmälan](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Använd inte kryssrutan för självbetjäning när du skapar SSL.

* **Befintliga SSL:er**: När du lägger till en domän söker systemet efter befintliga SSL:er, som kan ha skapats manuellt tidigare. Om du råkar ut för den här valideringen skapar du din domän utan att välja SSL-skapande, så ansluter vi dem åt dig. [Kontakta support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} om du vill ha mer information/alternativ.

* **Det går inte att lägga till certifikat till befintliga domäner**: Det går inte att lägga till certifikat till befintliga domäner just nu. För befintliga domäner, eller om du har missat att markera rutan för SSL-certifikat, måste du kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} för att få certifikatet tillagt.

* **Borttagning av domäner**: Om du tar bort en domän tas SSL-certifikatet bort automatiskt.
