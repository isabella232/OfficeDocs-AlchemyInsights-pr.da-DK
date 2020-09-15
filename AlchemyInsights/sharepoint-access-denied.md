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
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691677"
---
# <a name="troubleshoot-access-denied-messages"></a>Foretag fejlfinding af meddelelser om nægtet adgang

Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gennemse et SharePoint Online-websted, skal du se nedenstående artikler.

**Tilføje og licensere brugeren**

Kontrollér, at du [tildeler licenser til brugere i Microsoft 365 til virksomheder](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**Tildel tilladelser**

Hvis brugeren har fået tildelt en SharePoint-licens, og du stadig modtager en meddelelse om adgang nægtet, skal du sørge for, at de har de [relevante tilladelsesniveauer tildelt](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

**Overvej at bruge funktionen anmodning om adgang**

[Adgangs anmodnings](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) funktionen gør det muligt for personer at anmode om adgang til indhold, som de ikke aktuelt har tilladelse til at se. 

**Tillad, at brugerdefineret script muligvis får adgang til at nægte problemer**

Der er visse scenarier, hvor funktionen "Tillad brugerdefineret script" muligvis har adgang til at få adgang til at blive nægtet. Hvis du vil have en liste over funktioner, der er påvirket, sikkerhedsovervejelser og muligheden for at deaktivere funktionen. Besøg, [Tillad eller Forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Bemærk! Hvis et OneDrive-eller SharePoint-websted ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt tjeneste problem. [Se dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).


  

