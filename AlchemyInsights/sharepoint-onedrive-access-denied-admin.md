---
title: Fejlfinding i forbindelse med adgang nægtet-meddelelser
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751270"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Fejlfinding i forbindelse med adgang nægtet-meddelelser i SharePoint/OneDrive administration

Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gå til et SharePoint/OneDrive-administrations Center, skal du sørge for at [tildele brugeren en licens](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Hvis brugeren har en licens, skal du også sørge for, at de er [tildelt en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , der kan få adgang til administrations centrene.

Dette problem kan også opstå, når en bruger slettes og oprettes igen med det samme bruger hovednavn (UPN). Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. Et andet scenario involverer Katalogsynkronisering med en Active Directory-organisationsenhed (OU). Hvis brugerne allerede er logget på SharePoint, og de derefter flyttes til en anden OU og synkroniseres igen med SharePoint, kan de opleve dette problem.

Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Bemærk: Hvis et OneDrive-eller SharePoint-Administrationscenter ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt serviceproblem.  [Kontroller dashboardet for servicetilstand](https://portal.office.com/adminportal/home#/servicehealth).


