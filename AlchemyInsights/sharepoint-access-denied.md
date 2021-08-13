---
title: Fejlfinding af adgang nægtede meddelelser
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: af0bc0215f8feacc28a0b9bdf6b2659778736d669f7a3ff17628401e23d5fb6f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957967"
---
# <a name="troubleshoot-access-denied-messages"></a>Fejlfinding af adgang nægtede meddelelser

Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gennemse et Sharepoint Online-websted, skal du se nedenstående artikler.

**Tilføj og licenser brugeren**

Sørg for at [tildele licenser til brugere i Microsoft 365 til virksomheder.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)

**Tildel tilladelser**

Hvis brugeren har fået tildelt en SharePoint-licens og stadig modtager en meddelelse om adgang nægtet, skal du sikre dig, at brugeren har fået tildelt [det relevante tilladelsesniveau.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Overvej at bruge funktionen Adgangsanmodninger**

Funktionen [Adgangsanmodninger](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) giver brugerne mulighed for at anmode om adgang til indhold, som de ikke aktuelt har tilladelse til at se. 

**Tillad brugerdefineret script kan medføre problemer med adgang nægtet**

Der er visse scenarier, hvor funktionen "Tillad brugerdefineret script" muligvis præsenterer en adgang nægtet. For en liste over de funktioner, der er påvirket, sikkerhedsmæssige overvejelser og muligheden for at deaktivere funktionen. Besøg , Tillad [eller forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Bemærk! Hvis et OneDrive-SharePoint-websted ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et problem med en midlertidig tjeneste. [Kontrollér dashboardet over tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).


  

