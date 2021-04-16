---
title: Udfasning af Exchange PowerShell og basisgodkendelse
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813466"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="040a4-102">Udfasning af Exchange PowerShell og basisgodkendelse</span><span class="sxs-lookup"><span data-stu-id="040a4-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="040a4-103">Hvis du vil have de nyeste oplysninger om, hvordan du opretter forbindelse til Exchange Online PowerShell uden brug af basisgodkendelse, skal du [gå hertil](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="040a4-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="040a4-104">PowerShell V2-modulet bruger ikke basisgodkendelse.</span><span class="sxs-lookup"><span data-stu-id="040a4-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="040a4-105">Bemærk, at basisgodkendelse stadig skal være aktiveret på klientmaskinen.</span><span class="sxs-lookup"><span data-stu-id="040a4-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="040a4-106">Det nye PowerShell V2-modul bruger moderne godkendelse til at etablere forbindelse til at aktivere alle REST baserede v2-cmdletter.</span><span class="sxs-lookup"><span data-stu-id="040a4-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="040a4-107">Ud over v2-cmdletter giver det dig også mulighed for at få adgang til ældre Remote PowerShell (RPS)-cmdletter, som kræver, at der oprettes en Remote PowerShell-session.</span><span class="sxs-lookup"><span data-stu-id="040a4-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="040a4-108">Når du opretter en RPS-session på Windows-maskine, kræver det, at WinRM BasicAuth aktiveres på klientmaskinen, selvom modulet bruger moderne godkendelsesmekanisme til at godkende tjenesten.</span><span class="sxs-lookup"><span data-stu-id="040a4-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="040a4-109">WinRM Basic auth-pipelinen bruges til at transportere tokens til moderne godkendelse.</span><span class="sxs-lookup"><span data-stu-id="040a4-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="040a4-110">Hvis WinRM Basic auth er deaktiveret på klientmaskinen, vil de nye v2-cmdletter stadig fungere (men de ældre RPS-cmdletter vil ikke).</span><span class="sxs-lookup"><span data-stu-id="040a4-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
