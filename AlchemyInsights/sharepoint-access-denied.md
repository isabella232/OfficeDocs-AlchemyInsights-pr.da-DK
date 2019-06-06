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
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735732"
---
# <a name="troubleshoot-access-denied-messages"></a>Fejlfinding i forbindelse med meddelelser adgang nægtet

Hvis du modtager en adgang nægtet vises, når du forsøger at gennemse et Sharepoint Online-websted, skal du se i nedenstående artikler.

## <a name="add-and-license-the-user"></a>Tilføje og licens til brugeren

Sikre, at du [tildele licenser til brugere i Office 365 til virksomheder](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).

Tildele tilladelser

Hvis brugeren har fået tildelt en licens til Sharepoint og stadig modtager en meddelelse om nægtet adgang, Kontroller, at de har [tildelt passende tilladelsesniveau](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).

Overvej at bruge funktionen anmodning

[Anmodning om adgang](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) -funktion gør det muligt at anmode om adgang til indhold, de ikke har tilladelse til at se. 

Tillad brugerdefinerede script kan forårsage adgang nægtet problemer

Der er visse situationer, hvor funktionen "Tillad brugerdefineret script" kan give en adgang nægtet. For en liste over funktioner, der påvirkes, sikkerhedsovervejelser og muligheden for at deaktivere funktionen. Besøg, [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)

Bemærk: Hvis en OneDrive eller SharePoint-webstedet ikke er tilgængeligt for flere brugere, der tidligere havde adgang, kan der være et problem med den midlertidige tjeneste. [Kontroller service sundhed dashboardet](https://portal.office.com/adminportal/home#/servicehealth).


  

