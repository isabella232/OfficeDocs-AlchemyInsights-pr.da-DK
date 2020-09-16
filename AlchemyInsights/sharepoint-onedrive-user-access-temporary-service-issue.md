---
title: Problemer med ydeevnen – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771238"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive langsom, utilgængelig eller ikke tilgængelig for flere brugere

Hvis et OneDrive-eller SharePoint-websted ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt tjeneste problem. [Se dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).

**Tilføje og licensere brugeren**

Kontrollér, at du [tildeler licenser til brugere i Microsoft 365 til virksomheder](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tildel tilladelser**

Hvis brugeren har fået tildelt en SharePoint-licens, og du stadig modtager en meddelelse om adgang nægtet, skal du sørge for, at de har de [relevante tilladelsesniveauer](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tildelt.

**Overvej at bruge funktionen anmodning om adgang**

[Adgangs anmodnings funktionen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) gør det muligt for personer at anmode om adgang til indhold, som de ikke aktuelt har tilladelse til at se.

**Tillad, at brugerdefineret script muligvis får adgang til at nægte problemer**

Der er visse scenarier, hvor funktionen til *at aktivere brugerdefinerede scripts* muligvis har en adgang, der er nægtet. Hvis du vil have en liste over funktioner, der er påvirket, sikkerhedsovervejelser og muligheden for at deaktivere funktionen. Gå til [Tillad eller Forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

