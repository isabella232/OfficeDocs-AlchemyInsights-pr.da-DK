---
title: Tildeling af grupper til Azure AD-rolle
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036234"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Tildeling af grupper til Azure AD-rolle

Hvis du vil tildele en Azure AD-gruppe med kilde til autoritet i Azure AD til en Azure AD-rolle, skal du udføre følgende trin:

1. Opret en ny gruppe – Sådan opretter du en ny gruppe:

    a. Log på Azure AD Administration med rettigheder **som rolleadministrator** **eller global administrator.**
    b. Vælg **Azure Active Directory > Grupper > Alle grupper > Ny gruppe.**
    c. Opret gruppen.

2. Tildel rollen til gruppen enten under gruppeoprettelsen, eller når gruppen er oprettet.

    a. Hvis du vil tildele en rolle til gruppen på tidspunktet for gruppeoprettelsen, skal du slå **Azure AD-roller** til og fra og oprette gruppen.
    b. Hvis du vil tildele en rolle til gruppen,  efter den er blevet oprettet, skal du gå til fanen Tildelte roller for den nyoprettede gruppe og tildele rollen til gruppen.  

**Administrer medlemskab af en gruppe, der er tildelt en Azure AD-rolle**

For at forhindre udvidelse af rettigheder kan kun privilegerede rolleadministratorer og globale administratorer som standard ændre medlemskabet af en gruppe, der er tildelt en rolle. De kan dog vælge at tildele en ejer til en sådan gruppe og uddelegere denne opgave.

Hvis du vil have mere at vide om at tildele skygrupper til Azure AD-roller, skal du [se Tildel en AD-rolle til skygruppe](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Hvis du vil have mere at vide om fejlfinding af roller, der er tildelt til skygrupper, skal du [se Fejlfinding af roller, der er tildelt til skygrupper.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





