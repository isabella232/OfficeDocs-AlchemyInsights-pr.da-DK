---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833069"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="8e866-102">Fejlmeddelelsen "Beklager, en anden konto fra organisationen er allerede logget på" i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="8e866-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="8e866-103">Du kan rette fejlen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="8e866-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="8e866-104">Fjern alle arbejdskonti, undtagen den pågældende konto, ved hjælp af Windows-indstillinger > **Access til arbejde eller skole.**</span><span class="sxs-lookup"><span data-stu-id="8e866-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="8e866-105">[Ryd Office-legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) hjælp af Windows Legitimationsstyring.</span><span class="sxs-lookup"><span data-stu-id="8e866-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="8e866-106">**Bemærk!** Stierne i registreringsdatabasen til Office 2016 er ændret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="8e866-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8e866-107">(Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="8e866-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="8e866-108">Åbn en Office-app, og **vælg**  >  **Log af**  >  **filkonto.** Log derefter på med en brugerkonto med en gyldig licens.</span><span class="sxs-lookup"><span data-stu-id="8e866-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="8e866-109">Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8e866-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8e866-110">For Mac skal du se [Jeg kan ikke logge på en Office 2016 til Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="8e866-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="8e866-111">Du kan få mere at vide [under "Vi beklager, men en anden konto fra din organisation allerede er logget på denne computer" i Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="8e866-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>