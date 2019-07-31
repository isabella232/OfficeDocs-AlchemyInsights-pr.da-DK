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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938173"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="f2fcd-102">Fastsættelse af Office apps meddelelsen "Beklager, en anden konto fra organisationen allerede er logget på"</span><span class="sxs-lookup"><span data-stu-id="f2fcd-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="f2fcd-103">Du kan rette denne fejl, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="f2fcd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="f2fcd-104">Fjerne alle konti i arbejde, bortset fra den berørte konto ved hjælp af Windows-indstillinger > **Access arbejdet eller i skolen**.</span><span class="sxs-lookup"><span data-stu-id="f2fcd-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="f2fcd-105">[Fjern Office legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af styring af legitimationsoplysninger i Windows.</span><span class="sxs-lookup"><span data-stu-id="f2fcd-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f2fcd-106">**Bemærk:** Stier i registreringsdatabasen for Office 2016 er ændret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="f2fcd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f2fcd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f2fcd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="f2fcd-108">Åbn et Office-program, skal du vælge **filen** > **konto** > **Log af**. Log på ved hjælp af en brugerkonto med en gyldig licens.</span><span class="sxs-lookup"><span data-stu-id="f2fcd-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="f2fcd-109">Du kan finde detaljerede oplysninger [konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="f2fcd-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="f2fcd-110">Du [kan ikke logge på en Office-2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)til Mac.</span><span class="sxs-lookup"><span data-stu-id="f2fcd-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="f2fcd-111">Yderligere oplysninger finder du ["Desværre en anden konto fra organisationen allerede er logget på på denne computer" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="f2fcd-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>