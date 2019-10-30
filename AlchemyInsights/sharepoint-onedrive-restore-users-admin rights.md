---
title: Fejlfinding af adgang nægtet-meddelelser til OneDrive for Business-websteder
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766705"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Fejlfinding af adgang nægtet-meddelelser til OneDrive for Business-websteder

Dette problem opstår oftest, når en bruger slettes og oprettes igen med det samme bruger hovednavn (UPN). Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. Et andet scenario involverer Katalogsynkronisering med en Active Directory-organisationsenhed (OU). Hvis brugerne allerede er logget på SharePoint, og de derefter flyttes til en anden OU og synkroniseres igen med SharePoint, kan de opleve dette problem.

1. Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Hvis du ikke kan gendanne den oprindelige bruger, skal du fjerne den gamle bruger fra OneDrive-webstedet ved hjælp af disse trin, [fjerne en bruger fra listen brugeroplysninger](). 
3. Når dette er gjort, kan du kontrollere, at brugeren har administratorrettigheder til OneDrive-webstedet ved at følge trinnene for at [tilføje administrator's for en brugers onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Du finder flere oplysninger om tilladelsesniveauer i artiklen om [tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
