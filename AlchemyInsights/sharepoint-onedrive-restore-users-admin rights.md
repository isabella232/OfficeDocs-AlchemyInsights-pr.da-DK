---
title: Give brugere adgang til SharePoint og OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759250"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Give brugere adgang til SharePoint og OneDrive

Dette problem opstår oftest, når en bruger slettes og genoprettes med det samme brugerens hovednavn (UPN). Den nye konto er oprettet ved hjælp af en anden værdi af PUID (Passport Entydigt ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. Et andet scenario omfatter katalogsynkronisering med en Active Directory-organisationsenheden (OU). Hvis brugerne har allerede logget på SharePoint, og derefter er flyttet til en anden OU og resynced med SharePoint, kan de opleve dette problem.

Du kan løse dette problem skal du gendanne den oprindelige UPN med trinnene i artiklen,[gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Når dette er gjort, kan du kontrollere, at brugeren har admin-rettigheder til webstedet OneDrive ved at følge trinnene til [Tilføj admin's for en brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Du kan finde yderligere oplysninger om tilladelsesniveauer finder artikel, [forståelse af tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
