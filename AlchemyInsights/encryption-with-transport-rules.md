---
title: Kryptering med transportregler
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
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079444"
---
# <a name="encryption-with-transport-rules"></a>Kryptering med transportregler

I [Exchange Administration](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) kan du bruge funktionaliteterne i Office-meddelelseskryptering (OME) i forbindelse med reglerne for mailflow til at udløse meddelelseskryptering. Vælg indstillingen **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse** i betingelsen for transportreglen.

- Hvis du vil have mere at vide, skal du se [Definer regel for mailflow til kryptering af](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- I PowerShell skal du bruge [Ny – TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet og konfigurere parameteret *ApplyOME* til $true.
