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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743948"
---
# <a name="create-user"></a>Opret bruger

**MEDDELELSE:**

- [Udvisning af understøttelse af WebView-logon fra Google pr. 4. januar 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Test, om dine apps kan blive påvirket, ved [at følge Googles vejledning til](https://go.microsoft.com/fwlink/?linkid=2157323) test af kompatibilitet.
- Sørg for at bruge systemets webvisning eller systembrowser, når du logger på dine brugere med Google-forbrugerkonti. Du kan få mere at vide [under Problemer med kun at logge på programmer ved hjælp af Chrome-browseren.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Jeg kan ikke oprette en ny bruger i mit Azure AD-katalog**

1. Sørg for, at du er autoriseret til at oprette en ny standardbruger. Kun den globale administrator- eller brugeradministratorrolle i Azure Active Directory (AD) kan oprette en ny standardbruger. Hvis du ikke er i en af disse roller, kan du bede en administrator om at føje dig til en af disse roller eller oprette en ny brugerkonto for dig.
1. Sørg for, at brugernavnet er i et domæne, der er bekræftet i din Azure AD. Hvis du ikke har nogen bekræftede brugerdefinerede domænenavne i dit Azure AD, kan du bruge dit indledende Azure AD-domæne, som slutter med *.onmicrosoft.com.
1. Sørg for, at brugernavnet er i et domæne, der ikke er medlem af organisationsnetværket med Azure AD fra dit lokale AD. Brugere kan ikke tilføjes i skyen med domænenavne, der er medlem af organisationsnetværket i det lokale miljø.
1. Sørg for, at ingen andre brugere eller kontakter allerede har det brugernavn, du vil tildele den nye bruger. Brugernavne skal være entydige på tværs af Azure AD.
1. Se [Roller og administratorer for Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD for dit Azure AD.
1. Se [domænenavnene til](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) din Azure AD.
1. Gennemse [overvågningslogfiler for](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) at få vist mere detaljerede oplysninger om en nyligt oprettet eller slettet bruger, som f.eks. hvem der udførte handlingen og hvornår.
1. Du kan finde flere oplysninger om at tilføje nye [brugere i Brug Azure-portalen til at oprette en ny bruger i dit Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Administrative roller i Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Administratorrolletilladelser i Azure Active Directory
1. Du kan også [bruge Azure AD PowerShell til at oprette en ny bruger.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
