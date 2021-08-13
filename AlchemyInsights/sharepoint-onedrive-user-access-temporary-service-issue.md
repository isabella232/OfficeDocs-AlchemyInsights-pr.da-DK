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
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093687"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive, Ikke tilgængelig eller Utilgængelig for flere brugere

Hvis et OneDrive eller SharePoint websted ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt problem med tjenesten. [Kontrollér dashboardet over tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).

**Tilføj og licenser brugeren**

Sørg for at [tildele licenser til brugere i Microsoft 365 til virksomheder.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Tildel tilladelser**

Hvis brugeren har fået tildelt en SharePoint-licens og stadig modtager en meddelelse om adgang nægtet, skal du sikre dig, at brugeren har tildelt [det relevante tilladelsesniveau.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Overvej at bruge funktionen Adgangsanmodninger**

Funktionen [Adgangsanmodninger](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) giver brugerne mulighed for at anmode om adgang til indhold, som de ikke aktuelt har tilladelse til at se.

**Tillad brugerdefineret script kan medføre problemer med adgang nægtet**

Der er visse scenarier, hvor funktionen *Tillad brugerdefineret script* muligvis præsenterer en adgang nægtet. For en liste over de funktioner, der er påvirket, sikkerhedsmæssige overvejelser og muligheden for at deaktivere funktionen. Besøg Tillad [eller forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

