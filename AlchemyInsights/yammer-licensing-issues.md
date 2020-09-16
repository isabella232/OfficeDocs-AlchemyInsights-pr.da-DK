---
title: Problemer med Yammer-licens
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657270"
---
# <a name="yammer-licensing-issues"></a>Problemer med Yammer-licens

Alle brugere skal have en licens for at bruge Yammer Enterprise-tjenesten, men som standard kræver Yammer ikke, at brugere har en licens til at få adgang til tjenesten. Når en administrator ændrer indstillingen for at blokere Microsoft 365-brugere uden Yammer-licenser, har brugere, der ikke har fået tildelt en Yammer Enterprise-licens, ikke adgang til Yammer-tjenesten. Du kan finde flere oplysninger i [administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Når licenser fjernes fra brugerne, vises Yammer-feltet ikke længere, og andre tjenester kan bruge Fjern licens til at skjule funktioner. I andre tilfælde kan funktioner stadig vises, men kræver licenstildeling for at fungere.  

**Licensen bliver ikke opdateret for brugeren**  

Nogle gange tildeles en bruger en licens, men det er stadig ikke muligt at få adgang til Yammer. Der er større sandsynlighed for forsinkelser, når der er en masse licenstildeling i gang. Yammer-brugere opdateres muligvis ikke i samme rækkefølge, da licenser er ændret i Azure AD, fordi systemet kører asynkront. Vent op til 24 timer, før du åbner en support situation for at rapportere problemer med synkronisering af licenser.  

**Masse licenstildeling**  

Licenser kan tildeles via Administrationscenter eller PowerShell-scripting. Du kan få mere at vide under [Tildel licenser til brugere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og [Tildel licenser til brugerkonti med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft Support yder ikke hjælp til oprettelse af scripts, men dokumentation til Yammer-licenstildeling er tilgængelig. Du kan finde flere oplysninger i [administrere Yammer-licenser ved hjælp af Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).