---
title: Problemer med Yammer-licenser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148201"
---
# <a name="yammer-licensing-issues"></a>Problemer med Yammer-licenser

Alle brugere skal have licens til at bruge Yammer Enterprise-tjenesten, men Yammer kræver som standard ikke, at brugerne har licens til at få adgang til tjenesten. Når en administrator ændrer indstillingen for at blokere Microsoft 365-brugere uden Yammer-licenser, kan brugere, der ikke har fået tildelt en Yammer Enterprise-licens, ikke få adgang til Yammer-tjenesten. Du kan finde flere oplysninger under [Administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Når licenser fjernes fra brugere, vises Yammer-feltet ikke længere, og andre tjenester kan bruge fjernelse af licenser til at skjule funktioner. I andre tilfælde kan funktioner stadig vises, men kræver licenstildeling for at fungere.  

**Licensen opdateres ikke for brugeren**  

Af og til tildeles en bruger en licens, men kan stadig ikke få adgang til Yammer. Der er større sandsynlighed for forsinkelser, når en masselicenstildeling er i gang. Yammer-brugere opdateres muligvis ikke i samme rækkefølge, som licenser ændres i Azure AD, fordi systemet kører asynkront. Vent op til 24 timer, før du åbner en supportsag for at rapportere licenssynkroniseringsproblemer.  

**Masselicenstildeling**  

Licenser kan tildeles via Administration eller PowerShell-scripting. Du kan finde flere oplysninger under [Tildele licenser til brugere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og Tildele licenser til [brugerkonti med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft Support hjælper ikke med at oprette scripts, men dokumentation om Yammer-licenstildeling er tilgængelig. Du kan finde flere oplysninger under [Administrere Yammer-licenser ved hjælp af Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).