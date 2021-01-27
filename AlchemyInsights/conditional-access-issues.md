---
title: Betingede adgangsproblemer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014787"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="7e958-102">Betingede adgangsproblemer</span><span class="sxs-lookup"><span data-stu-id="7e958-102">Conditional access issues</span></span>

<span data-ttu-id="7e958-103">**Løse problemer med logon-diagnosticering**</span><span class="sxs-lookup"><span data-stu-id="7e958-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="7e958-104">Du kan hurtigt finde ud af, hvad der skete eller diagnosticere problemer i forbindelse med brugerlogon, ved hjælp af [logonsessionen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="7e958-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="7e958-105">Start den diagnosticering, du har logget på.</span><span class="sxs-lookup"><span data-stu-id="7e958-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="7e958-106">Find den hændelse, der skal analyseres, ved at angive de oplysninger, du har om bruger, program, tidspunkt for logon, anmodnings-id eller korrelations-id.</span><span class="sxs-lookup"><span data-stu-id="7e958-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="7e958-107">Gennemgå de diagnostiske resultater, der viser oplysninger om, hvad der skete, og hvilke handlinger du kan udføre for at foretage ændringer (hvis der er behov for ændringer).</span><span class="sxs-lookup"><span data-stu-id="7e958-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="7e958-108">**Trin til fejlfinding af et logon**</span><span class="sxs-lookup"><span data-stu-id="7e958-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="7e958-109">Gå til siden Azure AD-logonsiden.</span><span class="sxs-lookup"><span data-stu-id="7e958-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="7e958-110">Filtrere logon-programmer efter bruger, tidsinterval, program, status, klient-app osv.</span><span class="sxs-lookup"><span data-stu-id="7e958-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="7e958-111">Vælg en logonindstilling, og få vist fanen betinget adgang for at se, hvilke politikker der blev evalueret.</span><span class="sxs-lookup"><span data-stu-id="7e958-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="7e958-112">Klik på rækken for en politik for at få vist politik detaljerne og forstå, hvorfor den er anvendt.</span><span class="sxs-lookup"><span data-stu-id="7e958-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="7e958-113">**Værktøjer til fejlfinding af en politik for betinget adgang**</span><span class="sxs-lookup"><span data-stu-id="7e958-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="7e958-114">Med rapport baseret tilstand kan du evaluere en politik uden at påvirke brugerne.</span><span class="sxs-lookup"><span data-stu-id="7e958-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="7e958-115">Hvad hvis-værktøj gør det muligt at simulere logon-begivenheder og se, hvilke politikker der gælder.</span><span class="sxs-lookup"><span data-stu-id="7e958-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="7e958-116">Indsigt og rapporterings projektmapper viser realtids virkninger for hver politik.</span><span class="sxs-lookup"><span data-stu-id="7e958-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="7e958-117">**Grundlæggende beskyttelsespolitikker**</span><span class="sxs-lookup"><span data-stu-id="7e958-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="7e958-118">Grundlæggende beskyttelsespolitikker er blevet frarådet.</span><span class="sxs-lookup"><span data-stu-id="7e958-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="7e958-119">De håndhæves ikke længere og vil snart blive fjernet fra Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="7e958-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="7e958-120">Vi anbefaler, at du aktiverer [sikkerhedsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="7e958-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="7e958-121">Hvis du vil have mere at vide om betinget adgang, skal du se:</span><span class="sxs-lookup"><span data-stu-id="7e958-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="7e958-122">[Bedste fremgangsmåder for betinget adgang i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Betingelser i betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolelementer i betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Placeringer i betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="7e958-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
