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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557963"
---
# <a name="workflow-is-not-starting"></a>Arbejdsprocessen starter ikke

- Arbejdsgange i SharePoint 2010, og SharePoint 2013 starter ikke.

    - Hvis arbejdsprocessen ikke starter, kan der være et problem med den midlertidige tjeneste hvor brugere kan opleve forbigående forsinkelser med status for arbejdsprocessen. Kontroller [Service sundhed Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for at se, hvis organisationen påvirkes.

    - Hvis der er gået mere end 24 timer, da du så først problemet, skal du logge en støtte billet. I mange tilfælde kan arbejder vi allerede på en løsning. Giv os, mindst 24 timer at gennemføre en løsning.

- SharePoint 2010-arbejdsprocesser forsinkelse ved start.

    - Dette sker, hvis arbejdsprocessen udløses i store partier. (for eksempel, når flere elementer tilføjes på én gang).

    - Arbejdsprocesser er ikke beregnet til at køre i realtid, så en forsinkelse er tilsigtet funktionsmåde.

   -  Kompileringen kan være langsom, hvis arbejdsgangen er komplekse Extensible objekt Markup Language (XMOL). Læs [denne](https://support.microsoft.com/en-us/kb/3043697) artikel.

    - Du bør forenkle arbejdsgangen eller designe det ved hjælp af Microsoft SharePoint 2013 platform arbejdsgangstype.

    - Hvis din arbejdsgangshistorikken er blevet stort, kan du fjerne varerne eller oprette en ny oversigtsliste.

        Yderligere oplysninger: [Fjern arbejdsgangshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Relaterede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Oprette produktionsflow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


