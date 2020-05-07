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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Udfasning af Exchange PowerShell og basisgodkendelse

Hvis du vil have de nyeste oplysninger om, hvordan du opretter forbindelse til Exchange Online PowerShell uden brug af basisgodkendelse, skal du [gå hertil](https://aka.ms/psbasicauth).

Bemærk, at basisgodkendelse stadig skal være aktiveret på klientmaskinen.
Det nye PowerShell V2-modul bruger moderne godkendelse til at etablere forbindelse til at aktivere alle REST baserede v2-cmdletter. Ud over v2-cmdletter giver det dig også mulighed for at få adgang til ældre Remote PowerShell (RPS)-cmdletter, som kræver, at der oprettes en Remote PowerShell-session. Når du opretter en RPS-session på Windows-maskine, kræver det, at WinRM BasicAuth aktiveres på klientmaskinen, selvom modulet bruger moderne godkendelsesmekanisme til at godkende tjenesten. WinRM Basic auth-pipelinen bruges til at transportere tokens til moderne godkendelse. Hvis WinRM Basic auth er deaktiveret på klientmaskinen, vil de nye v2-cmdletter stadig fungere (men de ældre RPS-cmdletter vil ikke).
