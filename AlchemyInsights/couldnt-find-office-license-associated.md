---
title: Rettede Microsoft 365-apps Kunne ikke finde tilknyttede office-licenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580435"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="d91ee-102">Rettelse af Microsoft 365-apps "Kunne ikke finde tilknyttede kontorlicenser"</span><span class="sxs-lookup"><span data-stu-id="d91ee-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="d91ee-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="d91ee-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d91ee-104">Kontroller din firewall, dit antivirusprogram og dine proxyindstillinger for at bekræfte, at de ikke blokerer for internetadgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="d91ee-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d91ee-105">Se [Microsoft 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d91ee-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="d91ee-106">Fjern og [tildel Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) til den berørte bruger igen.</span><span class="sxs-lookup"><span data-stu-id="d91ee-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="d91ee-107">Åbn en Office-app, og [log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af eksisterende brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="d91ee-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="d91ee-108">Gå til Windows-indstillinger **Accounts**>  >  **konti, & konti,** og fjern alle arbejdskonti undtagen den berørte konto.</span><span class="sxs-lookup"><span data-stu-id="d91ee-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="d91ee-109">Gå til Windows-indstillinger > **Konti**  >  **Access-arbejde eller -skole**, og afbryd forbindelsen til alle arbejdskonti undtagen den berørte konto.</span><span class="sxs-lookup"><span data-stu-id="d91ee-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="d91ee-110">Nulstil office-aktiveringstilstanden.</span><span class="sxs-lookup"><span data-stu-id="d91ee-110">Reset the Office activation state.</span></span> <span data-ttu-id="d91ee-111">[Få mere at vide om, hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="d91ee-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="d91ee-112">[Log på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="d91ee-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="d91ee-113">Du kan finde flere fejlfindingsløsninger [under Produkt- og aktiveringsfejl uden licens i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="d91ee-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>