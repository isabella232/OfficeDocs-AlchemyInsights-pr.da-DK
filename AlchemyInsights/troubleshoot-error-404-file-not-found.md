---
title: Fejlfinding af fejl 404, filen blev ikke fundet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 5c65aabf41ca17c9164e3f167346d314bc4e92d47f5fc17c188f12819b0a2cfa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048546"
---
# <a name="troubleshoot-error-404-file-not-found"></a>Fejlfinding af fejl 404, filen blev ikke fundet

Fejlen 404 modtages, når brugere forsøger at få adgang til et websted eller en fil i SharePoint eller OneDrive. Dette skyldes ofte, at et websted eller en fil eller gruppe bliver omdøbt, flyttet eller slettet. For eksempel: Brugerne vil opleve en 404-fejl, der forsøger at få adgang til roden af gruppen af websteder, og den er blevet slettet.

Sådan løser du fejl 404 for et websted, der er blevet omdøbt, flyttet eller slettet:

For klassiske websteder, der findes i den klassiske Administration, skal du [se Gendan en slettet gruppe af websteder](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).

For moderne websteder (kommunikation, gruppeforbundne websteder eller andre websteder), der findes i den nye SharePoint Administration, skal du se Få vist og gendan slettede websteder [i den nye SharePoint Administration.](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

For at løse fejl 404 for en fil (eller et andet element), der er blevet omdøbt, flyttet eller slettet:

Gå til webstedet SharePoint eller OneDrive, og få vist Papirkurv fra webstedets indhold. Se [Gendan elementer i Papirkurv på et SharePoint websted](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).

Hvis du stadig ikke kan finde elementet, du kan søge i overvågningsloggen, hvis logføring er aktiveret, skal du se Søg i overvågningsloggen i [Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).
