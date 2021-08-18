---
title: Opret bruger
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323280"
---
# <a name="create-user"></a>Opret bruger

**MEDDELELSE:**

- [Udrådning af WebView-logonsupport fra Google fra den 4. januar 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Test, om dine apps kan blive påvirket, ved [at følge Googles vejledning til](https://go.microsoft.com/fwlink/?linkid=2157323) test af kompatibilitet.
- Sørg for at bruge systemwebvisningen eller systembrowseren, når du logger dine brugere på med Google-forbrugerkonti. Du kan få mere at vide [under Problemer med at logge på programmer, der kun bruger Chrome-browseren.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Jeg kan ikke oprette en ny bruger i mit Azure AD-katalog**

1. Sørg for, at du er godkendt til at oprette en ny standardbruger. Kun den globale administrator eller brugeradministratorrollen i Azure Active Directory (AD) kan oprette en ny standardbruger. Hvis du ikke er i en af disse roller, kan du bede en administrator om at føje dig til en af disse roller eller oprette den nye brugerkonto for dig.
1. Sørg for, at brugernavnet er i et domæne, der er bekræftet i din Azure AD. Hvis du ikke har nogen bekræftede brugerdefinerede domænenavne i dit Azure AD, kan du bruge dit indledende Azure AD-domæne, som slutter med *.onmicrosoft.com.
1. Sørg for, at brugernavnet er i et domæne, der ikke er i organisationsnetværk med Azure AD fra dit lokale AD. Brugere kan ikke tilføjes i skyen med domænenavne, der er medlem af organisationsnetværket i det lokale miljø.
1. Sørg for, at ingen andre brugere eller kontakter allerede har det brugernavn, du vil tildele den nye bruger. Brugernavne skal være entydige på tværs af Azure AD.
1. Se [Roller og administratorer i Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD for dit Azure AD.
1. Se [domænenavnene til](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) dit Azure AD.
1. Gennemse [overvågningslogfiler for at](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) få vist mere detaljerede oplysninger om en nyligt oprettet eller slettet bruger, som f.eks. hvem der udførte handlingen og hvornår.
1. Du kan finde flere oplysninger om at tilføje nye brugere [i Brug Azure-portalen til at oprette en ny bruger i dit Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal).
1. [Administrative roller i Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Administratorrolletilladelser i Azure Active Directory
1. Du kan også [bruge Azure AD PowerShell til at oprette en ny bruger.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
