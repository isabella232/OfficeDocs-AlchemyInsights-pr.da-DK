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
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="86434-102">Kryptering med transportregler</span><span class="sxs-lookup"><span data-stu-id="86434-102">Encryption with transport rules</span></span>

<span data-ttu-id="86434-103">I [Exchange Administration](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) kan du bruge funktionaliteterne i Office-meddelelseskryptering (OME) i forbindelse med reglerne for mailflow til at udløse meddelelseskryptering.</span><span class="sxs-lookup"><span data-stu-id="86434-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="86434-104">Vælg indstillingen **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse** i betingelsen for transportreglen.</span><span class="sxs-lookup"><span data-stu-id="86434-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="86434-105">Hvis du vil have mere at vide, skal du se [Definer regel for mailflow til kryptering af](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="86434-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="86434-106">I PowerShell skal du bruge [Ny – TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet og konfigurere parameteret *ApplyOME* til $true.</span><span class="sxs-lookup"><span data-stu-id="86434-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
