---
title: Arbejdsprocessen er ikke startet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907732"
---
# <a name="workflow-is-not-starting"></a>Arbejdsprocessen er ikke startet

- SharePoint 2010- SharePoint 2013-arbejdsprocesser startes ikke.

    - Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjenesteproblem, hvor brugere kan opleve forbigående forsinkelser i arbejdsprocesforløbet. Kontrollér [dashboardet Tjenestetilstand for](https://admin.microsoft.com/AdminPortal/Home/servicehealth) at se, om din organisation påvirkes.

    - Hvis der er gået mere end 24 timer, siden du så dette problem første gang, skal du logge en supportanmodning. I mange tilfælde arbejder vi allerede på en løsning. Giv os mindst 24 timer til at fuldføre en løsning.

- SharePoint 2010-arbejdsprocesser forsinket ved start.

    - Dette sker, hvis arbejdsprocessen udløses i store batches. (f.eks. når flere elementer tilføjes på én gang).

    - Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er designet til at være en god ide.

   -  Hvis arbejdsprocessen er kompleks Extensible Object Markup Language (X RESSOURCE), kan kompileringen være langsom. Se [denne](https://support.microsoft.com//kb/3043697) artikel.

    - Du bør forenkle arbejdsprocessen eller ændre dens design ved hjælp af platformtypen Microsoft SharePoint 2013-arbejdsproces.

    - Hvis arbejdsproceshistorikken er blevet stor, kan det være en god ide at fjerne elementerne eller oprette en ny oversigtsliste.

        Flere oplysninger: [Slette arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opret Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
