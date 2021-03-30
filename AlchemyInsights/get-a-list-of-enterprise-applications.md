---
title: Få en liste over Virksomhedsprogrammer
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404532"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="d723e-102">Få en liste over Virksomhedsprogrammer</span><span class="sxs-lookup"><span data-stu-id="d723e-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="d723e-103">Se  [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)for at få en liste over virksomhedsprogrammer (alle programmer eller filtreret efter vist navn, id, identifikator-URI'er osv.) via kommandoen Powershell.</span><span class="sxs-lookup"><span data-stu-id="d723e-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="d723e-104">Se [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)for at få en liste over tjenesteprincipalobjekter (alle objekter eller filtreret efter id) via Kommandoen Powershell.</span><span class="sxs-lookup"><span data-stu-id="d723e-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="d723e-105">Hvis du vil have **en liste over SAML-konfigurerede apps, kan følgende PowerShell-scripts** hjælpe dig:</span><span class="sxs-lookup"><span data-stu-id="d723e-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="d723e-106">Hvert program, uanset om det er en OAuth-app eller SAML-app (både galleriapps og ikke-galleriapps), har to objekter oprettet i AAD, når deres registrering sker.</span><span class="sxs-lookup"><span data-stu-id="d723e-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="d723e-107">Det ene kaldes programobjektet, og det andet er objektet Tjenesteinspektør.</span><span class="sxs-lookup"><span data-stu-id="d723e-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="d723e-108">Når du gemmer egenskaberne for et Tjeneste principal-objekt ved hjælp af PowerShell, vil du opdage, at hvert program har et bestemt antal mærker, der er knyttet til det, f.eks.:</span><span class="sxs-lookup"><span data-stu-id="d723e-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="d723e-109">OAuth-apps ville have et mærke kaldet "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="d723e-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="d723e-110">Gallery SAML Apps ville have et mærke kaldet "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="d723e-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="d723e-111">SAML-apps, der ikke er galleri, har et mærke med navnet "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="d723e-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="d723e-112">Derfor kan du bruge disse mærker og finde ud af, hvilken slags app det er.</span><span class="sxs-lookup"><span data-stu-id="d723e-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="d723e-113">Mærket "**WindowsAzureActiveDirectoryIntegratedApp**" er fælles for alle typer apps.</span><span class="sxs-lookup"><span data-stu-id="d723e-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="d723e-114">Du kan bruge følgende kodestykke til at få vist alle SAML-apps (både galleri og ikke-galleri):</span><span class="sxs-lookup"><span data-stu-id="d723e-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="d723e-115">Du kan finde flere oplysninger i [Identificer SAML-aktiverede apps i Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="d723e-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="d723e-116">**Find og vis kun webprogrammer:** Brug kommandoen nedenfor til at få alle Azure AD-programmer med programtypen "Webapp/API"</span><span class="sxs-lookup"><span data-stu-id="d723e-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="d723e-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="d723e-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="d723e-118">**Find og opliste kun oprindelige programmer:** Kør følgende kommando for at hente alle de oprindelige klientprogrammer (stationære computere/mobilenheder).</span><span class="sxs-lookup"><span data-stu-id="d723e-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="d723e-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="d723e-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="d723e-120">**Eksportér alle registrerede Azure AD-programoplysninger til CSV: Kommandoen** nedenfor eksporterer alle Azure AD-apps med obligatoriske oplysninger til CSV-filen:</span><span class="sxs-lookup"><span data-stu-id="d723e-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="d723e-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="d723e-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="d723e-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Kodning af UTF8</span><span class="sxs-lookup"><span data-stu-id="d723e-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="d723e-123">**Brug for at eksportere en liste over ubrugte Azure-apps** – Overvågningsrapport</span><span class="sxs-lookup"><span data-stu-id="d723e-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="d723e-124">Azure AD kan kun vise programlogfiler i op til 30 dage, hvis du har en Azure AD Premium-licens.</span><span class="sxs-lookup"><span data-stu-id="d723e-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="d723e-125">Du har to muligheder for at bevare dataene i mere end 30 dage.</span><span class="sxs-lookup"><span data-stu-id="d723e-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="d723e-126">Du kan bruge [API'er til Azure AD-rapportering](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) til at hente dataene ved hjælp af et program og gemme dem i en database.</span><span class="sxs-lookup"><span data-stu-id="d723e-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="d723e-127">Alternativt kan du integrere overvågningslogfiler i et TREDJEPARTS SIEM-system.</span><span class="sxs-lookup"><span data-stu-id="d723e-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="d723e-128">Du kan også downloade applisten for alle programmer og ejete programmer under Azure Active Directory>App-registreringer>Download>Alle programmer/ejet programmer.</span><span class="sxs-lookup"><span data-stu-id="d723e-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="d723e-129">Hvis du vil have en liste over programmer via MS Graph, skal du se [Listeprogrammer – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) og programressourcetype [– Microsoft Graph v1.0.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="d723e-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
