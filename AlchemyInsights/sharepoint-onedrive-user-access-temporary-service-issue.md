---
title: Problemer med ydeevne-SharePoint- eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719511"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint- eller OneDrive langsomt, utilgængelig eller ikke tilgængeligt for flere brugere

Hvis en OneDrive eller SharePoint-webstedet ikke er tilgængeligt for flere brugere, der tidligere havde adgang, kan der være et problem med den midlertidige tjeneste. [Kontroller service sundhed dashboardet](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Tilføje og licens til brugeren

Sikre, at du [tildele licenser til brugere i Office 365 til virksomheder](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Tildele tilladelser

Hvis brugeren har fået tildelt en licens til Sharepoint og stadig modtager en meddelelse om nægtet adgang, Kontroller, at de har [passende tilladelsesniveau](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) , der er tildelt.

## <a name="consider-using-the-access-request-feature"></a>Overvej at bruge funktionen anmodning

[Anmodning om funktion i access](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) gør det muligt at anmode om adgang til indhold, de ikke har tilladelse til at se.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Tillad brugerdefinerede script kan forårsage adgang nægtet problemer

Der er visse situationer, hvor funktionen *Tillad brugerdefineret script* kan være præsenterer en adgang nægtet. For en liste over funktioner, der påvirkes, sikkerhedsovervejelser og muligheden for at deaktivere funktionen. Besøg [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

