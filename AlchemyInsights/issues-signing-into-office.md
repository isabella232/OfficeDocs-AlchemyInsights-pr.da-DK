---
title: Problemer, der logger på Office apps
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938174"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="78092-102">Problemer, der logger på Office apps</span><span class="sxs-lookup"><span data-stu-id="78092-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="78092-103">For at løse problemer-logon med Office apps, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="78092-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="78092-104">Fjerne alle konti i arbejde, bortset fra den berørte konto ved hjælp af Windows-indstillinger > **Access arbejdet eller i skolen**.</span><span class="sxs-lookup"><span data-stu-id="78092-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="78092-105">[Fjern Office legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af styring af legitimationsoplysninger i Windows.</span><span class="sxs-lookup"><span data-stu-id="78092-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="78092-106">**Bemærk:** Stier i registreringsdatabasen for Office 2016 er ændret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="78092-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="78092-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="78092-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="78092-108">Åbn et Office-program, skal du vælge **filen** > **konto** > **Log af**. Log på ved hjælp af en brugerkonto med en gyldig licens.</span><span class="sxs-lookup"><span data-stu-id="78092-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="78092-109">Du kan finde detaljerede oplysninger [konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="78092-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="78092-110">Du [kan ikke logge på en Office-2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)til Mac.</span><span class="sxs-lookup"><span data-stu-id="78092-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="78092-111">Hvis der opstår fejl under oprettelse af forbindelse til Office 365 ved hjælp af Office-2013, skal du aktivere moderne godkendelse for Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="78092-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="78092-112">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="78092-112">For more information, see:</span></span>
- [<span data-ttu-id="78092-113">Du kan ikke logge på Office 365, Azure eller Intune</span><span class="sxs-lookup"><span data-stu-id="78092-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="78092-114">Forbindelsesproblemer i logon efter opdatering til Office 2016 bygge 16.0.7967 på Windows-10</span><span class="sxs-lookup"><span data-stu-id="78092-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="78092-115">"Undskyld, en anden konto fra organisationen allerede er logget på på denne computer" i Office</span><span class="sxs-lookup"><span data-stu-id="78092-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="78092-116">Fejlfinding af logonproblemer med moderne Office-godkendelse, når du bruge ADFS</span><span class="sxs-lookup"><span data-stu-id="78092-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)