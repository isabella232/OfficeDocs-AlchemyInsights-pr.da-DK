---
title: Meddelelse om, at Microsoft 365-apps ikke kunne finde de tilknyttede Office-licenser
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816482"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="9d451-102">Fejlmeddelelsen "Kunne ikke finde office-licenser tilknyttet" i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="9d451-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="9d451-103">Hvis du modtager denne meddelelse, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="9d451-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9d451-104">Kontrollér din firewall, din antivirussoftware og dine proxyindstillinger for at bekræfte, at de ikke blokerer internetadgang til Microsoft 365-apps.</span><span class="sxs-lookup"><span data-stu-id="9d451-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9d451-105">Se [URL-adresser og IP-adresseintervaller for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9d451-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="9d451-106">Fjern og [tildel Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den pågældende bruger igen.</span><span class="sxs-lookup"><span data-stu-id="9d451-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="9d451-107">Åbn en Office-app, [og log](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) af eventuelle eksisterende brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="9d451-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="9d451-108">Gå til Windows-indstillinger > **konti**  >  **& konti,** og fjern alle arbejdskonti undtagen den pågældende konto.</span><span class="sxs-lookup"><span data-stu-id="9d451-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="9d451-109">Gå til Windows-indstillinger **>-konti**  >  **Adgang til arbejde eller skole,** og afbryd forbindelsen til alle arbejdskonti undtagen den pågældende konto.</span><span class="sxs-lookup"><span data-stu-id="9d451-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="9d451-110">Nulstil Office-aktiveringstilstanden.</span><span class="sxs-lookup"><span data-stu-id="9d451-110">Reset the Office activation state.</span></span> <span data-ttu-id="9d451-111">[Lær hvordan.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="9d451-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="9d451-112">[Log på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den pågældende brugerkonto.</span><span class="sxs-lookup"><span data-stu-id="9d451-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="9d451-113">Du kan finde flere fejlfindingsløsninger [under Fejl i forbindelse med produkt og aktivering uden licens i Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="9d451-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>