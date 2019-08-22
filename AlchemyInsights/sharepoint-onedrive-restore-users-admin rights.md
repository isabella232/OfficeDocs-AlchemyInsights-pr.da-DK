---
title: Fejlfinding af ingen adgang meddelelser til OneDrive for Business-websteder
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507805"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Fejlfinding af ingen adgang meddelelser til OneDrive for Business-websteder

Dette problem opstår oftest, når en bruger slettes og genoprettes med det samme brugerens hovednavn (UPN). Den nye konto er oprettet ved hjælp af en anden værdi af PUID (Passport Entydigt ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. Et andet scenario omfatter katalogsynkronisering med en Active Directory-organisationsenheden (OU). Hvis brugerne har allerede logget på SharePoint, og derefter er flyttet til en anden OU og resynced med SharePoint, kan de opleve dette problem.

1. Du kan løse dette problem skal du gendanne den oprindelige UPN med trinnene i artiklen,[gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Hvis du ikke kan gendanne den oprindelige bruger, skal du fjerne den gamle bruger fra OneDrive-webstedet ved hjælp af disse trin, [fjerne en bruger fra brugerlisten info](). 
3. Når dette er gjort, kan du kontrollere, at brugeren har admin-rettigheder til webstedet OneDrive ved at følge trinnene til [Tilføj admin's for en brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Du kan finde yderligere oplysninger om tilladelsesniveauer finder artikel, [forståelse af tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
