---
title: Kontrollér automatiske opdateringer til Office-Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747770"
---
# <a name="control-automatic-updates-for-office-apps"></a>Kontrollér automatiske opdateringer til Office-Apps

Opdateringer til Office-apps downloades som standard automatisk og anvendes i baggrunden uden brugerinput. Administratorer kan dog styre, hvordan opdateringer anvendes ved hjælp af Office Update-indstillinger. Opdater indstillinger gør det muligt for administratorer at aktivere eller deaktivere automatiske opdateringer, vise eller skjule knappen **Opdater nu** i Office, angive deadlines og meget mere. Hvis du vil have mere at vide, skal du se:

- [Konfigurere opdateringsindstillinger for Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatisk opdatering til Office er ikke aktiveret](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definer, hvordan Office opdateres, efter det er installeret](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Hvis du vil gennemgå de eksisterende opdateringer, der er anvendt på en klientmaskine, skal du følge disse trin:

1. Åbn registrerings Editor ved at gå til **Start**  >  **kørsel**af  >  **regedit**.
2. Skift til følgende placering, og gennemse indstillingerne for Office Update:  
    a. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Bemærk!**  Hvis OfficeMgmtCOM-nøglen er angivet, får du muligvis vist meddelelsen "opdateringer administreres af din systemadministrator" i **Office**-  >  **kontoens**  >  **Office-opdateringer**. Du kan finde flere oplysninger i [administrere opdateringer til microsoft 365-apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  