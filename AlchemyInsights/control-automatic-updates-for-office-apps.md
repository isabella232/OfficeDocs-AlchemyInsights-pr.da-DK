---
title: Styre automatiske opdateringer til Office-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438992"
---
# <a name="control-automatic-updates-for-office-apps"></a>Styre automatiske opdateringer til Office-apps

Opdateringer til Office Apps hentes som standard automatisk og anvendes i baggrunden uden brugerindgriben. Administratorer kan dog styre, hvordan opdateringer anvendes, ved hjælp af Office Update-indstillinger. Opdateringsindstillinger giver administratorer mulighed for at aktivere eller deaktivere automatiske opdateringer, **vise eller skjule knappen Opdater** nu i Office, angive opdateringsfrister og meget mere. Yderligere oplysninger finder du i:

- [Konfigurere opdateringsindstillinger for Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatisk opdatering til Office er ikke aktiveret](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definere, hvordan Office opdateres, når det er installeret](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

FÃ ̧lg disse trin for at gennemse de eksisterende opdateringerindstillinger, der er anvendt på en klientcomputer:

1. Åbn Registreringseditor ved at gå **til Start**  >  **Kør**  >  **regedit**.
2. Skift til følgende placering, og gennemse indstillingerne for Office Update:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. Klik påRun\Konfiguration

**Bemærk:**  Hvis OfficeMgmtCOM-nøglen er angivet, vises meddelelsen "Opdateringer administreres af systemadministratoren" i **Office**  >  **Office-kontoopdateringer**  >  **Office Updates**. Du kan finde flere oplysninger [under Administrere opdateringer til Microsoft 365 Apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  