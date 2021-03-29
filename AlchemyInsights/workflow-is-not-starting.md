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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403737"
---
# <a name="workflow-is-not-starting"></a>Arbejdsprocessen er ikke startet

- SharePoint 2010- og SharePoint 2013-arbejdsprocesser starter ikke.

    - Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjenesteproblem, hvor brugere kan opleve forbigående forsinkelser med arbejdsprocesforløbet. Kontrollér [dashboardet Tjenestetilstand for](https://admin.microsoft.com/AdminPortal/Home/servicehealth) at se, om din organisation påvirkes.

    - Hvis der er gået mere end 24 timer, siden du så dette problem første gang, skal du logge en supportanmodning. I mange tilfælde arbejder vi allerede på en løsning. Giv os mindst 24 timer til at fuldføre en løsning.

- SharePoint 2010-arbejdsprocesser forsinket ved start.

    - Dette sker, hvis arbejdsprocessen udløses i store batches. (f.eks. når flere elementer tilføjes på én gang).

    - Arbejdsprocesser er ikke designet til at køre i realtid, så en forsinkelse er en designfunktion.

   -  Hvis arbejdsprocessen er kompleks Extensible Object Markup Language (XSUR), kan kompileringen være langsom. Se [denne](https://support.microsoft.com//kb/3043697) artikel.

    - Du bør forenkle arbejdsprocessen eller omdesigne den ved hjælp af microsoft SharePoint 2013-arbejdsprocesplatformtypen.

    - Hvis arbejdsproceshistorikken er blevet stor, kan det være en god ide at fjerne elementerne eller oprette en ny oversigtsliste.

        Flere oplysninger: [Slette arbejdsproceshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
