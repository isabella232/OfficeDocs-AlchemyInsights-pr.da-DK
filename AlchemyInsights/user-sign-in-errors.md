---
title: Fejl i bruger logger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900857"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="4422d-102">Fejl i bruger logger</span><span class="sxs-lookup"><span data-stu-id="4422d-102">User sign-in errors</span></span>

<span data-ttu-id="4422d-103">**Løse problemer med logon-diagnosticering**</span><span class="sxs-lookup"><span data-stu-id="4422d-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="4422d-104">Hvis du vil registrere årsagen eller diagnose problemer, der er relateret til brugerlogon, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="4422d-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="4422d-105">Start den [diagnosticering, du har logget på](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="4422d-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="4422d-106">Find den hændelse, der skal analyseres, ved at angive de oplysninger, du har om brugeren, programmet, klokkeslættet for logon, anmodnings-id eller korrelations-id.</span><span class="sxs-lookup"><span data-stu-id="4422d-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="4422d-107">Gennemgå de diagnostiske resultater, der viser oplysninger om, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer, hvis der er behov for ændringer.</span><span class="sxs-lookup"><span data-stu-id="4422d-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="4422d-108">**Leder du efter oplysninger om de AADSTS-fejlkoder, der returneres fra Azure Active Directory (Azure AD) sikkerhedstokentjenesten (STS)?**</span><span class="sxs-lookup"><span data-stu-id="4422d-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="4422d-109">Læs [denne artikel](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for at finde AADSTS-fejlbeskrivelser, rettelser og nogle forslag til løsninger</span><span class="sxs-lookup"><span data-stu-id="4422d-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>