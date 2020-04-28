---
title: Kryptering med transportregler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915089"
---
# <a name="encryption-with-transport-rules"></a>Kryptering med transportregler

I [Exchange Administration](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) kan du bruge funktionaliteterne i Office-meddelelseskryptering (OME) i forbindelse med reglerne for mailflow til at udløse meddelelseskryptering. Vælg indstillingen **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse** i betingelsen for transportreglen.

- Hvis du vil have mere at vide, skal du se [Definer regel for mailflow til kryptering af](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- I PowerShell skal du bruge [Ny – TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet og konfigurere parameteret *ApplyOME* til $true.
