---
title: Fejlfinding i forbindelse med meddelelser, der er nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758388"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Fejlfinding i forbindelse med adgang nægtet meddelelse i Sharepoint/OneDrive Administration

Hvis du modtager en meddelelse, der ikke er nægtet adgang, når du forsøger at gå til en Sharepoint/OneDrive Administration, skal du kontrollere, at du [tildeler en licens til brugeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Hvis brugeren har en licens, skal du også sikre dig, at vedkommende [tildeles en administratorrolle,](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) der kan få adgang til administratorcentrene.

Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme brugernavn (UPN). Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID. Et andet scenarie omfatter katalogsynkronisering med en Active Directory-organisationsenhed. Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden afdeling og synkroniseres igen med SharePoint, kan de opleve dette problem.

Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen [Gendan en bruger i Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Bemærk: Hvis et OneDrive eller SharePoint Administration ikke er tilgængeligt for flere brugere, der tidligere havde adgang, kan der være et midlertidigt tjenesteproblem.  [Tjek dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).


