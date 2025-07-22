---
unique-page-id: 2360185
description: Ändra säkerhetsinställningarna för lösenord - Marketo Docs - produktdokumentation
title: Ändra lösenordsinställningarna
exl-id: cda7ec70-32aa-4e0a-86b2-eb9bea70ef72
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Ändra lösenordsinställningarna {#change-your-password-security-settings}

Kontrollera lösenordsprincipen för din prenumeration. Så här gör du.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/change-your-password-security-settings-1.png)

1. Klicka på **[!UICONTROL Login Settings]**.

   ![](assets/change-your-password-security-settings-2.png)

1. Klicka på **[!UICONTROL Security Settings]** under **[!UICONTROL Edit]**.

   ![](assets/change-your-password-security-settings-3.png)

1. Välj en **[!UICONTROL Template]**. Om du vill ha avancerade alternativ klickar du på listrutan **[!UICONTROL Advanced]**.

   ![](assets/change-your-password-security-settings-4.png)

   >[!NOTE]
   >
   >En mall är bara en färdig konfiguration. **[!UICONTROL Standard Security]** är bra. **[!UICONTROL High Security]** är störst. Med **[!UICONTROL Custom]** kan du skapa egna.

   >[!TIP]
   >
   >I **[!UICONTROL Custom]** markerar du rutorna för att ange vilka egenskaper du vill att användarna ska ta med när de skapar lösenord.

1. Ange **[!UICONTROL Expiration]**. Den här funktionen kräver automatiskt att användarna återställer sina lösenord efter en viss tid. Detta gäller även administratören.

   ![](assets/change-your-password-security-settings-5.png)

   >[!CAUTION]
   >
   >Befintliga användare meddelas inte om ändringarna. Ange först **[!UICONTROL Expiration]** till 30 dagar för att säkerställa att alla har uppdaterat till de nya inställningarna och sedan ändra tillbaka detta till din ursprungliga cadence.

1. Ange **[!UICONTROL Inactive Session Timeout]**. Detta avgör hur länge en användare kan vara inaktiv innan han/hon måste logga in på Marketo igen.

   ![](assets/change-your-password-security-settings-6.png)
