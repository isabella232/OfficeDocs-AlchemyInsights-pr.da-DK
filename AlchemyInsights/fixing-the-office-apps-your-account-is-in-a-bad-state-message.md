---
title: Rettelse af Microsoft 365-apps Din konto er i en dårlig tilstand
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580111"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="74dc8-102">Rettelse af Microsoft 365-apps "Din konto er i en dårlig tilstand"</span><span class="sxs-lookup"><span data-stu-id="74dc8-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="74dc8-103">Du kan rette denne fejl ved at prøve følgende indstillinger på den berørte computer:</span><span class="sxs-lookup"><span data-stu-id="74dc8-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="74dc8-104">Åbn en Office-app, og vælg **Log**af  >  **filkonto**  >  **for alle konti**.</span><span class="sxs-lookup"><span data-stu-id="74dc8-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="74dc8-105">Log på igen ved hjælp af en brugerkonto med en gyldig licens.</span><span class="sxs-lookup"><span data-stu-id="74dc8-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="74dc8-106">Hvis du vil have mere at vide, skal du se [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="74dc8-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="74dc8-107">[Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Legitimationsstyring.</span><span class="sxs-lookup"><span data-stu-id="74dc8-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="74dc8-108">**Bemærk:** Registreringsdatabasen stier for Office 2016 er ændret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="74dc8-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="74dc8-109">\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="74dc8-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="74dc8-110">Hvis fejlen opstår under oprettelse af forbindelse til Office 365 ved hjælp af Office 2013, [skal du aktivere moderne godkendelse](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="74dc8-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="74dc8-111">Du kan finde flere oplysninger under [Sådan foretages fejlfinding af apps, der ikke er browsere, og som ikke kan logge på Microsoft 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="74dc8-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

