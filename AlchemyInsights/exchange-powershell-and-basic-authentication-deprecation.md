---
title: Udfasning af Exchange PowerShell og basisgodkendelse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015683"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="1a5d3-102">Udfasning af Exchange PowerShell og basisgodkendelse</span><span class="sxs-lookup"><span data-stu-id="1a5d3-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="1a5d3-103">Hvis du vil have de nyeste oplysninger om, hvordan du opretter forbindelse til Exchange Online PowerShell uden brug af basisgodkendelse, skal du [gå hertil](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="1a5d3-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="1a5d3-104">Bemærk, at basisgodkendelse stadig skal være aktiveret på klientmaskinen.</span><span class="sxs-lookup"><span data-stu-id="1a5d3-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="1a5d3-105">Det nye PowerShell V2-modul bruger moderne godkendelse til at etablere forbindelse til at aktivere alle REST baserede v2-cmdletter.</span><span class="sxs-lookup"><span data-stu-id="1a5d3-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="1a5d3-106">Ud over v2-cmdletter giver det dig også mulighed for at få adgang til ældre Remote PowerShell (RPS)-cmdletter, som kræver, at der oprettes en Remote PowerShell-session.</span><span class="sxs-lookup"><span data-stu-id="1a5d3-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="1a5d3-107">Når du opretter en RPS-session på Windows-maskine, kræver det, at WinRM BasicAuth aktiveres på klientmaskinen, selvom modulet bruger moderne godkendelsesmekanisme til at godkende tjenesten.</span><span class="sxs-lookup"><span data-stu-id="1a5d3-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="1a5d3-108">WinRM Basic auth-pipelinen bruges til at transportere tokens til moderne godkendelse.</span><span class="sxs-lookup"><span data-stu-id="1a5d3-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="1a5d3-109">Hvis WinRM Basic auth er deaktiveret på klientmaskinen, vil de nye v2-cmdletter stadig fungere (men de ældre RPS-cmdletter vil ikke).</span><span class="sxs-lookup"><span data-stu-id="1a5d3-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
