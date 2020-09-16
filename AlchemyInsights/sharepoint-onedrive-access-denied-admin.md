---
title: Foretag fejlfinding af meddelelser om nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767654"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Foretag fejlfinding af meddelelser om nægtet adgang i SharePoint/OneDrive administration

Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gå til en SharePoint/OneDrive administration, skal du sørge for, at du [tildeler en licens til brugeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Hvis brugeren har en licens, skal du også sørge for, at den er [tildelt en administratorrolle](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , der kan få adgang til administrations centrene.

Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme UPN-navn (User Principal Name). Den nye konto oprettes ved hjælp af en anden PUID-værdi (entydigt Passport-ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. En anden situation omfatter Katalogsynkronisering med en Active Directory-afdeling. Hvis brugerne allerede har logget på SharePoint, og de derefter flyttes til en anden OU og synkroniseres med SharePoint, kan de opleve dette problem.

For at løse dette problem skal du gendanne den oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Bemærk! Hvis en OneDrive-eller SharePoint-Administrationscenter ikke er tilgængelig for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt tjeneste problem.  [Se dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).


