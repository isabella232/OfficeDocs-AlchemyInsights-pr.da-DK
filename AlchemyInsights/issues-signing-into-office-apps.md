---
title: Problemer med at logge på Microsoft 365-apps
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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579859"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="9dd47-102">Rettelse af Microsoft 365-apps "Computerens platformsmodul, der er tillid til, fungerer ikke korrekt"</span><span class="sxs-lookup"><span data-stu-id="9dd47-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="9dd47-103">Du kan rette fejlen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="9dd47-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="9dd47-104">Installer de nyeste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9dd47-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9dd47-105">[Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Legitimationsstyring.</span><span class="sxs-lookup"><span data-stu-id="9dd47-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9dd47-106">**Bemærk:** Registreringsdatabasen stier for Office 2016 er ændret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="9dd47-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9dd47-107">(Eks.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9dd47-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="9dd47-108">Prøv [brugergenoprettelsesprocessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for at rette TPM-fejl (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="9dd47-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="9dd47-109">Angiv EnableADAL = 0 ved hjælp af følgende trin:</span><span class="sxs-lookup"><span data-stu-id="9dd47-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="9dd47-110">Højreklik på knappen Start i Windows, vælg **Kør**, skriv **regedit**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="9dd47-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="9dd47-111">Vælg **Ja** for at tillade, at Registreringseditor foretager ændringer på enheden.</span><span class="sxs-lookup"><span data-stu-id="9dd47-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="9dd47-112">Tilføj en DWORD-værdi i **EnableADAL** i Registreringseditor med en indstilling **på 0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="9dd47-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="9dd47-113">Du kan finde flere oplysninger [under Forbindelsesproblemer ved logon efter opdatering til Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9dd47-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>