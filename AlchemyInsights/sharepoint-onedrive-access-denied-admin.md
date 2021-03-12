---
title: Fejlfinding af adgang nægtet meddelelser
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707948"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Fejlfinding af adgang nægtet meddelelser i Sharepoint/OneDrive Administration

Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gå til en Sharepoint/OneDrive Administration, skal du sørge for at tildele en licens [til brugeren.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Hvis brugeren har en licens, skal du også sikre dig, at de [er tildelt en administratorrolle,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) der kan få adgang til Administration.

Dette problem kan også opstå, når en bruger slettes og genoprettes med samme brugerens hovednavn (UPN). Den nye konto oprettes ved hjælp af en anden værdi for PUID (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID. Et andet scenarie indebærer katalogsynkronisering med en Active Directory-organisationsenhed (OU). Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden OU og synkroniseres igen med SharePoint, kan de opleve dette problem.

Du kan løse dette problem ved at gendanne det oprindelige UPN ved hjælp af trinnene i artiklen Gendan [en bruger i Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Bemærk! Hvis en OneDrive- eller SharePoint Administration ikke er tilgængelig for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt problem med tjenesten.  [Kontrollér dashboardet over tjenestetilstand.](https://portal.office.com/adminportal/home#/servicehealth)


