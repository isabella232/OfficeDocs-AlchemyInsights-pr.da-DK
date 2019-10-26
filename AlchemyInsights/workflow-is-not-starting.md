---
title: Arbejdsprocessen starter ikke
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738083"
---
# <a name="workflow-is-not-starting"></a>Arbejdsprocessen starter ikke

- Arbejdsprocesser i SharePoint 2010 og SharePoint 2013 starter ikke.

    - Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt serviceproblem, hvor brugerne kan opleve periodiske forsinkelser med status for arbejdsprocessen. Kontroller [dashboardet for tjenestetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation påvirkes.

    - Hvis der er gået mere end 24 timer, siden du så dette problem, skal du logge en support billet. I mange tilfælde arbejder vi allerede på en løsning. Giv os mindst 24 timer til at gennemføre en løsning.

- SharePoint 2010-arbejdsprocesser forsinket på Start.

    - Dette sker, hvis arbejdsprocessen udløses i store batches. (f. eks. Når flere elementer tilføjes på én gang).

    - Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er efter design-opførsel.

   -  Hvis arbejdsprocessen er komplekst Extensible Object Markup Language (XMOL), kan kompileringen være langsom. Tjek [denne](https://support.microsoft.com//kb/3043697) artikel.

    - Du bør forenkle arbejdsprocessen eller ændre den ved hjælp af Microsoft SharePoint 2013-arbejdsproces platforms typen.

    - Hvis din Arbejdsproceshistorik er blevet større, kan du slette emnerne eller oprette en ny oversigtsliste.

        Flere oplysninger: [rydde Arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


