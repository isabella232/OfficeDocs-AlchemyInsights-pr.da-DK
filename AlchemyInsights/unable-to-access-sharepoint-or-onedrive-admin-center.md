---
title: Kan ikke få adgang SharePoint eller OneDrive Administration
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020438"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Kan ikke få adgang SharePoint eller OneDrive Administration

- Hvis webstedet SharePoint eller OneDrive Administration ikke er tilgængeligt eller utilgængeligt, kan der være et midlertidigt tjenesteproblem, hvor brugerne oplever forbigående forsinkelser eller navigationsfejl, når de får adgang til SharePoint websteder eller OneDrive indhold. Kontrollér [dashboardet Tjenestetilstand for](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) at se, om din organisation påvirkes.

- Globale og SharePoint administratorer skal have tildelt en SharePoint licens. Nyligt oprettede konti, der netop er tildelt en SharePoint-licens eller administratorrolle, kan opleve problemer med at få adgang til SharePoint, f.eks. "adgang nægtet" eller "brugeren blev ikke fundet". Giv mindst 24 timer, før synkroniseringen er fuldført på tværs af vores systemer. Vi forstår, at 24 timer kan se ud som lang tid. I mange tilfælde arbejder vi allerede på en løsning.

- Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) brugere kan få adgang nægtet, hvis vinduet med tilladelse til at få adgang er meget lille, se Adgang nægtet [til PIM-konti](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).