---
title: Fastsættelse af Office-apps Din konto er i en meddelelse om dårlig tilstand
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969341"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="c4912-102">Rette op på Office-appsene "Din konto er i dårlig tilstand"-fejl</span><span class="sxs-lookup"><span data-stu-id="c4912-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="c4912-103">Du kan løse denne fejl ved at prøve følgende indstillinger på den berørte computer:</span><span class="sxs-lookup"><span data-stu-id="c4912-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="c4912-104">Åbn en Office-app, vælg Log på **filer** > **konto** > **af alle konti**.</span><span class="sxs-lookup"><span data-stu-id="c4912-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="c4912-105">Log på igen ved hjælp af en brugerkonto med en gyldig licens.</span><span class="sxs-lookup"><span data-stu-id="c4912-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="c4912-106">Du kan finde detaljerede oplysninger under [Konti i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c4912-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c4912-107">[Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="c4912-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="c4912-108">**Bemærk:** Registreringsdatabasestierne for Office 2016 er ændret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="c4912-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c4912-109">\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="c4912-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="c4912-110">Angiv EnableADAL = 0 på den berørte computer ved hjælp af følgende trin:</span><span class="sxs-lookup"><span data-stu-id="c4912-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="c4912-111">Højreklik på Windows-knappen, og vælg **Kør**.</span><span class="sxs-lookup"><span data-stu-id="c4912-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="c4912-112">Skriv **regedit**i feltet **Åbn** , og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="c4912-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="c4912-113">Vælg **Ja,** når du bliver bedt om at tillade, at Registreringseditor foretager ændringer på enheden.</span><span class="sxs-lookup"><span data-stu-id="c4912-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="c4912-114">Tilføj en DWORD-værdi for EnableADAL i Registreringseditor med en indstilling på 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="c4912-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="c4912-115">Hvis fejlen opstår under oprettelse af forbindelse til Office 365 ved hjælp af Office 2013, skal du [aktivere moderne godkendelse](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) af Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="c4912-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="c4912-116">Du kan finde flere oplysninger under [Sådan foretages fejlfinding af apps, der ikke er browsere, og som ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="c4912-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

