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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539926"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="cf038-102">401 Uautoriseret fejl i SharePoint</span><span class="sxs-lookup"><span data-stu-id="cf038-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="cf038-103">Hvis du modtager fejlen "(401) uautoriseret" i SharePoint kan det være relateret til udrådningen af TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="cf038-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="cf038-104">For at få mere at vide, kan du se:</span><span class="sxs-lookup"><span data-stu-id="cf038-104">For more info, see:</span></span>

- [<span data-ttu-id="cf038-105">Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="cf038-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="cf038-106">Godkendelsesfejl opstår, hvis klienten ikke har understøttelse af TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="cf038-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="cf038-107">Opdater for at aktivere TLS 1.1 og TLS 1.2 som standard sikre protokoller i WinHTTP Windows</span><span class="sxs-lookup"><span data-stu-id="cf038-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="cf038-108">Hvis brugerne er på Windows 7, skal du kontrollere, at de markerer [TLS Cipher Suites i Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="cf038-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>