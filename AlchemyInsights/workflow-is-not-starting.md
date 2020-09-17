---
title: Arbejdsprocessen starter ikke
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794761"
---
# <a name="workflow-is-not-starting"></a>Arbejdsprocessen starter ikke

- SharePoint 2010-og SharePoint 2013-arbejdsprocesser starter ikke.

    - Hvis arbejdsprocessen ikke starter, kan der være et midlertidigt tjeneste problem, hvor brugerne kan opleve periodiske forsinkelser med arbejdsprocesstatus. Se [dashboardet for tjenestetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, om din organisation er påvirket.

    - Hvis der er gået mere end 24 timer, siden du først fik dette problem, skal du logge på en support billet. I mange tilfælde arbejder vi allerede på en løsning. Giv os mindst 24 timer for at fuldføre en løsning.

- SharePoint 2010-arbejdsprocesser forsinkede start.

    - Dette sker, hvis arbejdsprocessen udløses i store batches. (f. eks. Når flere elementer tilføjes på én gang).

    - Arbejdsprocesser er ikke beregnet til at køre realtid, så en forsinkelse er en funktionsmåde.

   -  Hvis arbejdsprocessen er komplekst XMOL (Extensible Object Markup Language), kan kompileringen være langsom. Se [denne](https://support.microsoft.com//kb/3043697) artikel.

    - Du bør forenkle arbejdsprocessen eller ændre designet ved hjælp af Microsoft SharePoint 2013 workflow platform-typen.

    - Hvis din Arbejdsproceshistorik er blevet stor, kan det være en god ide at slette elementerne eller oprette en ny oversigtsliste.

        Flere oplysninger: [rydde oversigt over arbejdsprocesser](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft flow i SharePoint Online?
- [Opret flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


