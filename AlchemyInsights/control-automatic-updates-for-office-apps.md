---
title: Styr automatiske opdateringer til Office apps
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
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929875"
---
# <a name="control-automatic-updates-for-office-apps"></a>Styr automatiske opdateringer til Office apps

Opdateringer til apps Office som standard automatisk og anvendes i baggrunden uden brugerindgreb. Administratorer kan dog styre, hvordan opdateringer anvendes, ved hjælp Office indstillingerne For opdatering. Opdateringsindstillinger gør det muligt for administratorer at  aktivere eller deaktivere automatiske opdateringer, vise eller skjule knappen Opdater nu i Office angive opdateringsdeadlines og meget mere. Hvis du vil have mere at vide, skal du se:

- [Konfigurere opdateringsindstillinger for Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatisk opdatering til Office ikke aktiveret](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definer, hvordan Office opdateres, når den er installeret](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Hvis du vil gennemgå de eksisterende opdateringsindstillinger, der er anvendt på en klientcomputer, skal du følge disse trin:

1. Åbn registreringseditoren ved at **gå til Start**  >  **Kør**  >  **regedit**.
2. Skift til følgende placering, og gennemse Office Opdater indstillinger:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Bemærk!**  Hvis OfficeMgmtCOM-nøglen er angivet, vises meddelelsen "Opdateringer administreres af din systemadministrator" muligvis **i Office**  >  **Account**  >  **Office Updates.** Du kan få mere at [vide under Administrer opdateringer Microsoft 365 Apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  