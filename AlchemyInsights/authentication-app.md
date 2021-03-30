---
title: Godkendelsesapp
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404597"
---
# <a name="authentication-app"></a><span data-ttu-id="73a70-102">Godkendelsesapp</span><span class="sxs-lookup"><span data-stu-id="73a70-102">Authentication app</span></span>

<span data-ttu-id="73a70-103">Hvis du er global administrator, kan du hurtigt finde ud af, hvad der skete, eller diagnosticere problemer relateret til brugerlogning ved hjælp af [Logondiagnosticering.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="73a70-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="73a70-104">Start diagnosticeringen ved at klikke på knappen "[Start diagnosticering".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="73a70-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="73a70-105">Find den hændelse, du vil analysere, ved at angive de oplysninger, du har om brugeren, programmet, tidspunktet for logon, anmodnings-id eller korrelations-id.</span><span class="sxs-lookup"><span data-stu-id="73a70-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="73a70-106">Gennemgå de diagnostiske resultater, der viser detaljer om, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer, hvis der er behov for ændringer.</span><span class="sxs-lookup"><span data-stu-id="73a70-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="73a70-107">**Kontrollér det scenarie, der er relevant:**</span><span class="sxs-lookup"><span data-stu-id="73a70-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="73a70-108">Hvis en bruger ikke får en pushmeddelelse i Microsoft Authenticator-appen, skal du bekræfte, at de ikke vises under de MFA-blokerede brugere som beskrevet i Bloker og fjerne [blokeringen af brugere.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="73a70-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="73a70-109">Hvis brugeren ikke er blokeret for MFA, men ikke modtager en pushmeddelelse, kan brugeren åbne Microsoft Authenticator-appen, som trækker de ventende godkendelsesanmodninger.</span><span class="sxs-lookup"><span data-stu-id="73a70-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="73a70-110">Som alternativ logonmetode kan brugeren også klikke på Log på en anden måde og vælge at bruge en bekræftelseskode fra min mobilapp.</span><span class="sxs-lookup"><span data-stu-id="73a70-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="73a70-111">Microsoft Authenticator-appen er den eneste tilgængelige metode for mange brugere.</span><span class="sxs-lookup"><span data-stu-id="73a70-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="73a70-112">[Få mere at vide om sikkerhedsstandard,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)se [Ofte stillede spørgsmål om Authenticator-appen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for ofte stillede spørgsmål, og hvordan du kan løse dem.</span><span class="sxs-lookup"><span data-stu-id="73a70-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="73a70-113">**Anbefalede videoer**</span><span class="sxs-lookup"><span data-stu-id="73a70-113">**Recommended Videos**</span></span>

<span data-ttu-id="73a70-114">[Sådan konfigurerer du Authenticator-appen på en ny telefon (2 minutter).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="73a70-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
