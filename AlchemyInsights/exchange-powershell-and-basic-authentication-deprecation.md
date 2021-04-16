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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Udfasning af Exchange PowerShell og basisgodkendelse

Hvis du vil have de nyeste oplysninger om, hvordan du opretter forbindelse til Exchange Online PowerShell uden brug af basisgodkendelse, skal du [gå hertil](https://aka.ms/exops-docs). PowerShell V2-modulet bruger ikke basisgodkendelse.

Bemærk, at basisgodkendelse stadig skal være aktiveret på klientmaskinen.
Det nye PowerShell V2-modul bruger moderne godkendelse til at etablere forbindelse til at aktivere alle REST baserede v2-cmdletter. Ud over v2-cmdletter giver det dig også mulighed for at få adgang til ældre Remote PowerShell (RPS)-cmdletter, som kræver, at der oprettes en Remote PowerShell-session. Når du opretter en RPS-session på Windows-maskine, kræver det, at WinRM BasicAuth aktiveres på klientmaskinen, selvom modulet bruger moderne godkendelsesmekanisme til at godkende tjenesten. WinRM Basic auth-pipelinen bruges til at transportere tokens til moderne godkendelse. Hvis WinRM Basic auth er deaktiveret på klientmaskinen, vil de nye v2-cmdletter stadig fungere (men de ældre RPS-cmdletter vil ikke).
