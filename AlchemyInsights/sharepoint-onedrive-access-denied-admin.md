---
title: Fejlfinding i forbindelse med meddelelser adgang nægtet
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503521"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Fejlfinding i forbindelse med adgang nægtet meddelelser i Sharepoint/OneDrive Admin Center

Hvis du modtager en adgang nægtet vises, når du forsøger at gå til administrationssiden for en Sharepoint/OneDrive, skal du kontrollere, at du [tildeler en licens til brugeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Hvis brugeren har en licens, skal du også sikre dig de er [tildelt en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , der kan få adgang til admin centrum.

Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme brugerens hovednavn (UPN). Den nye konto er oprettet ved hjælp af en anden værdi af PUID (Passport Entydigt ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. Et andet scenario omfatter katalogsynkronisering med en Active Directory-organisationsenheden (OU). Hvis brugerne har allerede logget på SharePoint, og derefter er flyttet til en anden OU og resynced med SharePoint, kan de opleve dette problem.

Du kan løse dette problem, skal du gendanne den oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Bemærk: Hvis en OneDrive eller SharePoint Administration center ikke er tilgængelig for flere brugere, som tidligere har haft adgang, kan der være et problem med den midlertidige tjeneste.  [Kontroller service sundhed dashboardet](https://portal.office.com/adminportal/home#/servicehealth).


