---
title: Find manglende programmer på bladet Til registrering af apps
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404413"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Find manglende programmer på bladet Til registrering af apps

1. Kan ikke finde programmer på appregistreringsportalen.

    Hvis et program er et program med flere lejere, og det er registreret i en anden lejer, vises det ikke under appregistreringsbladet. Du kan dog finde den under Enterprise Applications-bladet, når den er blevet åbnet (efter at have fået tilladelse), og tjenesteinspektøren er blevet oprettet i din lejer. Du kan få mere at vide [under Apps & tjeneste principaler i Azure AD – Microsoft Identity Platform.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Det er ikke muligt at få vist apps i siden Appregistrering, selvom du er administrator.

    Sørg for, at du er i den rigtige mappe på Azure-portalen.
3. Mit program er ikke angivet under Enterprise Applications-bladet, men det vises, når jeg forespørger om PowerShell-kommandoen.

    Nogle gange, når du sletter programmet fra Azure-portalen, vises det ikke på portalen, men det er muligvis ikke blevet slettet helt. Du kan finde flere oplysninger under:
    - Du kan hente listen over tidligere slettede programmer og se, om programmet vises på listen ved hjælp af **Powershell-kommandoen: Get-AzureADDeletedApplication.** Du kan få mere at [vide under Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Hvis du vil fjerne programmet helt, kan du prøve følgende i PowerShell: **Remove-AzureADApplication -ObjectId.** Du kan få mere at [vide under Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Alternativt kan du prøve at gendanne det slettede program ved hjælp af følgende Powershell-kommando: **Gendan AzureADDeletedApplication -ObjectId.** Du kan få mere at [vide under Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Jeg kan ikke finde en liste over alle forudinstallerede virksomhedsprogrammer i min nye Azure-lejer.

    Der er ingen forudinstallerede virksomhedsprogrammer i Azure AD som standard. Du skal tilføje det manuelt fra indstillingen "Nyt program" ved at gennemse det fra Azure AD-galleriet eller tilføje et program, der ikke er et galleri. Hvis du vil have mere at vide, [skal du se Quickstart: Føj et program til din Azure Active Directory-lejer (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Hvis du er global administrator, kan du nemt få adgang til dine apps ved hjælp [af Microsoft 365-appstarteren.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Kan ikke finde mine apps fra portalen Mine apps.

    Sørg for, at apps ikke er skjult på samlingssiden Mine apps. Du kan få mere at [vide under Samlinger (forhåndsvisning) på portalen Mine apps - Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Hvis du vil starte apps fra portalen Mine apps, skal du [se Finde & bruge apps på portalen Mine apps – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Mover-appen vises ikke på Enterprise Applications-bladet efter installationen.

    Programmet "Office 365 Mover" er en flertensiv app, der ikke behøver at være føjet til AAD ved hjælp af sektionen Galleriprogrammer under Enterprise App Registration. For at få adgang til Office 365 Mover-appen skal du blot logge på appen, så beder den om brugerens samtykke til tilladelserne. Når brugeren giver samtykke, føjes denne app automatisk til lejeren med det mail-id, du har logget på.

    Når du er logget på programmet, bør du kunne finde dette program under Enterprise Applications' blade i AAD. Du skal søge efter det pågældende program ved enten at skrive det fulde navn, dvs. "Office 365 Mover" eller ved blot at søge efter "office", og så skal appen angives. Hvis du vil have mere at vide, skal du se [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)og fortæller, at det allerede er installeret, men at det ikke er angivet i galleriet med virksomhedsprogram.
8. Hurtig start: Få vist listen over programmer, der bruger din [Azure Active Directory-lejer (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) til identitetsadministration, og se, hvordan du får vist de programmer, også kaldet apps, der allerede er konfigureret til at bruge din Azure AD-lejer som deres identitetsudbyder (IdP).
9. [Fejlfinding af almindelige problemer med at tilføje eller fjerne et program](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) til Azure Active Directory hjælper dig med at forstå de almindelige problemer, som brugere kan have med at få vist apps i Azure Active Directory.
