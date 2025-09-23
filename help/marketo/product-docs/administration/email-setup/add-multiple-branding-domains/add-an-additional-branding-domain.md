---
unique-page-id: 11377395
description: Lägg till en extra varumärkesdomän - Marketo Docs - produktdokumentation
title: Lägg till en extra varumärkesdomän
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Lägg till en extra varumärkesdomän {#add-an-additional-branding-domain}

Lägg till en extra varumärkesdomän när du kör flera varumärken från en enda Marketo-instans och vill att de ska ha sina egna varumärkesspårningslänkar.

>[!PREREQUISITES]
>
>Du måste [ersätta den generiska spårningslänken](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} med en profilerad domän innan du lägger till ytterligare profilerade domäner.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Klicka på **[!UICONTROL Add]** om du vill lägga till ytterligare en varumärkesdomän.

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. Ange namnet på den nya profileringsdomänen, välj _Gör primär domän_ och/eller _Generera SSL-certifikat_ (båda valfria) och klicka på **[!UICONTROL Save]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Gör primär domän_: Gör den här domänen till primär domän, och ange alla befintliga e-postmeddelanden som inte har skickats till &quot;Standard&quot; så används den primära domänen som standard för alla nya e-postmeddelanden. Du kan [skriva över detta per e-post](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Skapa SSL-certifikat_: Du kan skapa ett SSL-lager (Secure Sockets Layer) när du skapar domänen. Den första spårningsdomänen initierar en engångsinställning av infrastrukturen som kan ta några timmar. Du meddelas när allt är klart och du kan sedan konfigurera den första domänen. Om du vill lägga till SSL i dina befintliga domäner kan du kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Redigera SSL:er för befintliga domäner

Följ de här stegen för att aktivera SSL för dina befintliga domäner.

1. Välj _[!UICONTROL Admin]_&#x200B;i området **[!UICONTROL Email]**.

1. Markera domänraden på fliken _[!UICONTROL Domain]_&#x200B;och klicka på&#x200B;**[!UICONTROL Add SSL]**.

   ![Admin - E-post - Domän - Lägg till SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. Klicka på **[!UICONTROL Confirm]** i dialogrutan.

   ![Lägg till SSL - Bekräfta](./assets/generate-ssl-cert-confirm.png){width="400"}

## Felmeddelanden {#error-messages}

<table><thead>
  <tr>
    <th>Fel</th>
    <th>Information</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>Domänen finns redan.</i></td>
    <td>Det finns redan en domän med samma namn.</td>
  </tr>
  <tr>
    <td><i>Domänen är inte mappad till standarddomänen.</i></td>
    <td>Den anpassade domänen är inte korrekt mappad till standarddomänen. Kontrollera inställningarna för domänmappning och se till att DNS-konfigurationen pekar på rätt standarddomän.</td>
  </tr>
  <tr>
    <td><i>Det gick inte att utfärda SSL-certifikat på grund av CAA-poster som inte stöds. Begär att din IT-avdelning uppdaterar dina CAA-poster.</i></td>
    <td>CAA-posterna är inte uppdaterade. För dem som använder Marketo Engage hanterade SSL-certifikat måste CAA-posterna uppdateras till certifikat som rekommenderas av vår leverantör. Kontakta din IT-avdelning för att uppdatera CAA-posterna. Mer information finns på <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">den här sidan</a>.</td>
  </tr>
  <tr>
    <td><i>SSL-certifikatet har redan utfärdats.</i></td>
    <td>Det finns redan ett SSL-certifikat för den här anpassade domänen. Ingen ytterligare åtgärd krävs såvida inte certifikatet har upphört att gälla eller behöver utfärdas på nytt.</td>
  </tr>
  <tr>
    <td><i>Det gick inte att hitta standarddomänen. Kontakta supporten om du behöver hjälp.</i></td>
    <td>Det uppstod ett problem när standarddomänen skulle hittas. Kontakta supporten så att de kan undersöka saken.</td>
  </tr>
  <tr>
    <td><i>Ett oväntat fel uppstod när en domän skapades. Kontakta supporten om du behöver hjälp.</i></td>
    <td>Ett oväntat fel har inträffat. Hämta loggar och felinformation och eskalera problemet till <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo Support</a>.</td>
  </tr>
</tbody></table>

## Saker att notera {#things-to-note}

* **DNS-mappning för domän till Marketo Engage**: Innan du lägger till domäner i användargränssnittet måste du [mappa CNAME:er till en domän som tillhandahålls av Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Anpassade SSL:er**: Om du behöver en anpassad SSL:er skickar du en [supportanmälan](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Använd inte kryssrutan för självbetjäning när du skapar SSL.

* **Befintliga SSL:er**: När du lägger till en domän söker systemet efter befintliga SSL:er, som kan ha skapats manuellt tidigare. Om du råkar ut för den här valideringen skapar du din domän utan att välja SSL-skapande, så ansluter vi dem åt dig. [Kontakta support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} om du vill ha mer information/alternativ.

* **Borttagning av domäner**: SSL-certifikatet tas inte bort när domänen **tas bort automatiskt.** Skyddsplanen förhindrar användarfel som gör att en webbplats saknar SSL-certifikat. [Kontakta support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} om du vill ta bort SSL-certifikaten.

>[!MORELIKETHIS]
>
>[Redigera din standardprofileringsdomän](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
