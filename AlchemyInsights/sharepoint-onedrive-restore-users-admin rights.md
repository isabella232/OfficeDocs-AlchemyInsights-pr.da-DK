---
title: Foretage fejlfinding af adgang nægtet meddelelser til OneDrive for Business-websteder
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670610"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Foretage fejlfinding af adgang nægtet meddelelser til OneDrive for Business-websteder

Dette problem opstår ofte, når en bruger slettes og genoprettes med det samme UPN-navn (User Principal Name). Den nye konto oprettes ved hjælp af en anden PUID-værdi (entydigt Passport-ID). Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID. En anden situation omfatter Katalogsynkronisering med en Active Directory-afdeling. Hvis brugerne allerede har logget på SharePoint, og de derefter flyttes til en anden OU og synkroniseres med SharePoint, kan de opleve dette problem.

1. For at løse dette problem skal du gendanne det oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Hvis du ikke kan gendanne den oprindelige bruger, skal du fjerne den gamle bruger fra OneDrive-webstedet ved hjælp af disse trin, [Fjern en bruger fra listen brugeroplysninger](). 
3. Når dette er gjort, kan du bekræfte, at brugeren har administratorrettigheder til OneDrive-webstedet ved at følge trinnene til at [føje administratorerne til en brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Du kan finde flere oplysninger om tilladelsesniveauer i artiklen [om tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
