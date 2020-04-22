---
title: Arbejdsprocessen starter ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766091"
---
# <a name="workflow-is-not-starting"></a>Arbejdsprocessen starter ikke

- SharePoint 2010- og SharePoint 2013-arbejdsprocesser starter ikke.

    - Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjenesteproblem, hvor brugerne kan opleve periodiske forsinkelser med arbejdsgangens fremdrift. [Kontrollér Dashboardet for tjenestetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation er påvirket.

    - Hvis der er gået mere end 24 timer, siden du første gang så dette problem, skal du logge en supportbillet. I mange tilfælde arbejder vi allerede på en løsning. Giv os mindst 24 timer til at fuldføre en løsning.

- SharePoint 2010-arbejdsprocesser forsinket ved start.

    - Dette sker, hvis arbejdsprocessen udløses i store batches. (f.eks. når der tilføjes flere elementer på én gang).

    - Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er adfærd svære design.

   -  Hvis arbejdsprocessen er kompleks XMOL (Extensible Object Markup Language), kan kompileringen være langsom. Tjek [denne](https://support.microsoft.com//kb/3043697) artikel.

    - Du bør forenkle arbejdsprocessen eller ændre den ved hjælp af typen Af Typen af Microsoft SharePoint 2013 Workflow-platform.

    - Hvis arbejdsgangsoversigten er blevet stor, kan det være en god ide at fjerne elementerne eller oprette en ny oversigtsliste.

        Flere oplysninger : [Fjern arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


