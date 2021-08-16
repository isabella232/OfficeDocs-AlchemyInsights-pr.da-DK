---
title: Yammer problemer med licenser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989723"
---
# <a name="yammer-licensing-issues"></a>Yammer problemer med licenser

Alle brugere skal have licens til at bruge Yammer Enterprise-tjenesten, men som standard kræver Yammer ikke, at brugerne har en licens til at få adgang til tjenesten. Når en administrator ændrer indstillingen til at blokere Microsoft 365-brugere uden Yammer-licenser, kan brugere, der ikke er tildelt en Yammer Enterprise-licens, ikke få adgang til Yammer-tjenesten. Du kan finde flere oplysninger [i Yammer administrere brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Når licenser fjernes fra brugere, vises feltet Yammer ikke længere, og andre tjenester kan bruge fjernelse af licens til at skjule funktioner. I andre tilfælde kan funktioner stadig vises, men kræver tildeling af licens for at kunne fungere.  

**Licensen opdateres ikke for brugeren**  

Nogle gange tildeles en bruger en licens, men kan stadig ikke få adgang til Yammer. Der er større sandsynlighed for forsinkelser, når en masselicenstildeling er i gang. Yammer brugere muligvis ikke opdateres i samme rækkefølge, som licenser ændres i Azure AD, fordi systemet kører asynkront. Vent i op til 24 timer, før du åbner en supportsag for at rapportere problemer med licenssynkronisering.  

**Massetildeling af licens**  

Licenser kan tildeles via Administration eller PowerShell-scripting. Få mere at vide under [Tildel licenser til brugere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og [Tildel licenser til brugerkonti med Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsoft Support yder ikke hjælp til oprettelse af scripts, men dokumentationen om Yammer licenstildeling er tilgængelig. Du kan få mere at vide [under Administrere Yammer licenser ved hjælp af Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).