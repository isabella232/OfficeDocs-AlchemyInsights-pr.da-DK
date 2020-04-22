---
title: Problemer med at logge på Office-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762977"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="23f78-102">Problemer med at logge på Office-apps</span><span class="sxs-lookup"><span data-stu-id="23f78-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="23f78-103">Hvis du vil løse logonproblemer med Office-apps, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="23f78-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="23f78-104">Fjern alle arbejdskonti, undtagen den berørte konto, ved hjælp af Windows-indstillinger > **Access-arbejde eller skole**.</span><span class="sxs-lookup"><span data-stu-id="23f78-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="23f78-105">[Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="23f78-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="23f78-106">**Bemærk:** Registreringsdatabasestierne til Office 2016 er ændret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="23f78-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="23f78-107">(F.eks.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="23f78-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="23f78-108">Åbn en Office-app, og vælg**Log af** **filkonto** > **Account** > . Log derefter på med en brugerkonto med en gyldig licens.</span><span class="sxs-lookup"><span data-stu-id="23f78-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="23f78-109">Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="23f78-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="23f78-110">For Mac skal du se [Jeg kan ikke logge på en Office 2016 til Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="23f78-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="23f78-111">Hvis fejlene opstår under oprettelse af forbindelse til Microsoft 365 ved hjælp af Office 2013, skal du aktivere moderne godkendelse af Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="23f78-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="23f78-112">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="23f78-112">For more information, see:</span></span>
- [<span data-ttu-id="23f78-113">Du kan ikke logge på Microsoft 365, Azure eller Intune</span><span class="sxs-lookup"><span data-stu-id="23f78-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="23f78-114">Forbindelsesproblemer i logon efter opdatering til Office 2016 build 16.0.7967 på Windows 10</span><span class="sxs-lookup"><span data-stu-id="23f78-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="23f78-115">"Beklager, en anden konto fra din organisation er allerede logget på denne computer" i Office</span><span class="sxs-lookup"><span data-stu-id="23f78-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="23f78-116">Fejlfinding i forbindelse med logonproblemer med moderne Office-godkendelse, når du bruger ADFS</span><span class="sxs-lookup"><span data-stu-id="23f78-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)