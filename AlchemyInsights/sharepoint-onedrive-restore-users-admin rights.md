---
title: Fejlfinding af adgang nægtet meddelelser OneDrive for Business websteder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957787"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Fejlfinding af adgang nægtet meddelelser OneDrive for Business websteder

Dette problem opstår oftest, når en bruger slettes og genoprettes med samme brugerens hovednavn (UPN). Den nye konto oprettes ved hjælp af en anden VÆRDI for PUID (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID. Et andet scenarie omfatter katalogsynkronisering med en Active Directory-organisationsenhed (OU). Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden OU og synkroniseres med SharePoint, kan de opleve dette problem.

1. Du kan løse dette problem ved at gendanne det oprindelige UPN ved hjælp af trinnene i artiklen [Gendan en bruger Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Hvis du ikke kan gendanne den oprindelige bruger, skal du fjerne den gamle bruger fra OneDrive-webstedet ved hjælp af disse trin, Fjern en bruger fra [listen Brugeroplysninger.]() 
3. Når dette er gjort, kan du bekræfte, at brugeren har administratorrettigheder til OneDrive-webstedet ved at følge trinnene for at Tilføje administratorer for en [brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Du kan finde flere oplysninger om tilladelsesniveauer i artiklen [Om tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
