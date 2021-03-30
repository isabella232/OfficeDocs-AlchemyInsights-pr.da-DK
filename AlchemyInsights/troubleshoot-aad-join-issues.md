---
title: Fejlfinding af problemer med Azure AD-joinforbindelse
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404629"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="c0656-102">Fejlfinding af problemer med Azure AD-joinforbindelse</span><span class="sxs-lookup"><span data-stu-id="c0656-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="c0656-103">Hvis du konfigurerer enhedsregistreringer for første gang, skal du kontrollere, at du har gennemgået Introduktion til enhedshåndtering i [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) der kan hjælpe dig med at få enheder under kontrol til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0656-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="c0656-104">Hvis du registrerer enheder direkte i Azure AD og tilmelder dem i Intune, skal du først sikre [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) dig, at du har konfigureret [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) og licensering.</span><span class="sxs-lookup"><span data-stu-id="c0656-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="c0656-105">Sørg for, at du er autoriseret til at udføre handlinger i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0656-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="c0656-106">Kun en global administrator i Azure AD kan administrere indstillingerne for enhedsregistreringer.</span><span class="sxs-lookup"><span data-stu-id="c0656-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="c0656-107">Hvis du vil udføre implementering af Azure AD-joinforbindelse, skal [du se Planlæg Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="c0656-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="c0656-108">Hvis du vil have mere at vide om at løse almindelige problemer med Azure AD-joinforbindelse, skal du se Ofte stillede spørgsmål om [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) og for Windows 10 Pro-enhed. Kan ikke deltage i Windows [10 Pro-maskine](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) i Azure AD – skal opgraderes til – Microsoft Community</span><span class="sxs-lookup"><span data-stu-id="c0656-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
