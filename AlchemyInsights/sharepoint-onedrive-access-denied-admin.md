---
title: Fejlfinding i forbindelse med meddelelser om adgang nægtet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505373"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Fejlfinding i forbindelse med meddelelser om adgang nægtet i Sharepoint/OneDrive Administration

Hvis du modtager en meddelelse om adgang, der nægtes, når du forsøger at gå til et Sharepoint/OneDrive Administration, skal du sørge for at [tildele en licens til brugeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Hvis brugeren har en licens, skal du også sikre dig, at brugeren [tildeles en administratorrolle,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) der kan få adgang til administrationscentrene.

Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme brugernavn (UPN). Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID. Et andet scenarie omfatter katalogsynkronisering med en Active Directory-organisationsenhed. Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden afdeling og synkroniseres igen med SharePoint, kan de opleve dette problem.

Du kan lÃ ̧se problemet ved at gendanne den oprindelige UPN med trinnene i [artiklen, Gendan en bruger i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Bemærk: Hvis et OneDrive eller SharePoint Administration ikke er tilgængeligt for flere brugere, der tidligere havde adgang, kan der være et midlertidigt serviceproblem.  [Tjek dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).


