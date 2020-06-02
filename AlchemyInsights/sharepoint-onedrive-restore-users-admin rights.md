---
title: Fejlfinding i forbindelse med adgang til afviste meddelelser til OneDrive for Business-websteder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511178"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Fejlfinding i forbindelse med adgang til afviste meddelelser til OneDrive for Business-websteder

Dette problem opstår oftest, når en bruger slettes og genoprettes med det samme brugernavn (UPN). Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID. Et andet scenarie omfatter katalogsynkronisering med en Active Directory-organisationsenhed. Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden afdeling og synkroniseres igen med SharePoint, kan de opleve dette problem.

1. Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen ved [at gendanne en bruger i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Hvis du ikke kan gendanne den oprindelige bruger, skal du fjerne den gamle bruger fra OneDrive-webstedet ved hjælp af disse trin, [skal du fjerne en bruger fra listen over brugeroplysninger](). 
3. Når dette er gjort, kan du bekræfte, at brugeren har administratorrettigheder til OneDrive-webstedet ved at følge trinnene til [Tilføj administrator for en brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Yderligere oplysninger om tilladelsesniveauer finder du i artiklen [Om tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
