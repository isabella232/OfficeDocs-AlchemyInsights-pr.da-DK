---
title: 401 Uautoriseret fejl i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233492"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="5e296-102">401 Uautoriseret fejl i SharePoint</span><span class="sxs-lookup"><span data-stu-id="5e296-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="5e296-103">Hvis du modtager fejlen "(401) uautoriseret" i SharePoint kan det være relateret til udrådningen af TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="5e296-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="5e296-104">For at få mere at vide, kan du se:</span><span class="sxs-lookup"><span data-stu-id="5e296-104">For more info, see:</span></span>

[<span data-ttu-id="5e296-105">Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="5e296-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="5e296-106">Godkendelsesfejl opstår, hvis klienten ikke har understøttelse af TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="5e296-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="5e296-107">Hvis brugerne er på Windows 7, skal du kontrollere, at de markerer [TLS Cipher Suites i Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="5e296-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>