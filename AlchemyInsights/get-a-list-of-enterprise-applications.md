---
title: Få en liste over virksomhedsprogrammer
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116722"
---
# <a name="get-a-list-of-enterprise-applications"></a>Få en liste over virksomhedsprogrammer

1. Hvis **du** vil have en liste over virksomhedsprogrammer (alle programmer eller filtreret efter vist navn, id, id-URI'er osv.) via Powershell-kommandoen, skal du se [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Se [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)for at få en liste over tjenesteprincipalobjekter (alle objekter eller filtreret efter id) via kommandoen Powershell.
3. Hvis du vil have **en liste over SAML-konfigurerede apps, kan følgende PowerShell-scripts** hjælpe dig:

    Hvert program, uanset om det er en OAuth-app eller SAML-app (både galleriapps og ikke-galleriapps), har to objekter oprettet i AAD, når deres registrering sker. Det ene kaldes Programobjekt, og det andet er objektet Tjenesteinspektør. Når du gemmer egenskaberne for et tjeneste principal-objekt ved hjælp af PowerShell, vil du opdage, at hvert program har et bestemt antal mærker, der er knyttet til det, f.eks.:

    - OAuth-apps ville have et mærke med navnet "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps ville have et mærke med navnet "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - SAML-apps, der ikke er galleriet, har et mærke med navnet "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Derfor kan du bruge disse mærker og finde ud af, hvilken slags app det er. Mærket "**WindowsAzureActiveDirectoryIntegratedApp**" er fælles for alle typer apps. Du kan bruge følgende kodestykke til at få vist alle SAML-apps (både galleri og ikke-galleri):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Få mere at vide under [Identificer SAML-aktiverede apps i Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Find og vis kun webprogrammer:** Brug kommandoen nedenfor til at hente alle Azure AD-programmer med programtypen "Webapp/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Find og vis kun oprindelige programmer:** Kør følgende kommando for at få alle de oprindelige klientprogrammer (computer/mobilenhed).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Eksportér alle oplysninger om registreret Azure AD-program til CSV:** Kommandoen nedenfor eksporterer alle Azure AD-apps med de påkrævede oplysninger til CSV-filen:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Kodning af UTF8

7. **Brug for at eksportere en liste over ubrugte Azure-apps** – overvågningsrapport

    Azure AD kan kun vise programlogfiler i op til 30 dage, hvis du har Azure AD Premium licens.
    Du har to muligheder for at bevare dataene i mere end 30 dage. Du kan bruge [API'er til Azure AD-rapportering](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) til at hente dataene ved hjælp af et program og gemme dem i en database. Alternativt kan du integrere overvågningslogfiler i et SIEM-system fra tredjepart.

    Du kan også downloade applisten for alle programmer og ejet programmer under Azure Active Directory>Appregistreringer>Download>Alle programmer/ejet programmer.

    Hvis du vil have en liste over programmer via MS Graph, skal du se Listeprogrammer [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) og programressourcetype [– Microsoft Graph v1.0.](https://docs.microsoft.com/graph/api/resources/application)
