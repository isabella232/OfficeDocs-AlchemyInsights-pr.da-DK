---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709100"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="3a3ef-102">Meddelelse om, at din computers pålidelige platformsmodul ikke fungerer korrekt, i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="3a3ef-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="3a3ef-103">Du kan rette fejlen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="3a3ef-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="3a3ef-104">Installér de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="3a3ef-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="3a3ef-105">[Fjern Office-legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) hjælp af Windows Legitimationsstyring.</span><span class="sxs-lookup"><span data-stu-id="3a3ef-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3a3ef-106">**Bemærk!** Stierne i registreringsdatabasen til Office 2016 er ændret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="3a3ef-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3a3ef-107">(Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3a3ef-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3a3ef-108">Prøv processen [for brugergendannelse for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) at rette fejl i et platformsmodul (Trusted Platform Module, TPM).</span><span class="sxs-lookup"><span data-stu-id="3a3ef-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="3a3ef-109">Angiv EnableADAL = 0 ved at benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="3a3ef-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="3a3ef-110">Højreklik på knappen Start i Windows, vælg **Kør,** skriv **regedit,** og vælg derefter **OK.**</span><span class="sxs-lookup"><span data-stu-id="3a3ef-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="3a3ef-111">Vælg **Ja for** at tillade Registreringseditor at foretage ændringer på din enhed.</span><span class="sxs-lookup"><span data-stu-id="3a3ef-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="3a3ef-112">I Registreringseditor skal du tilføje en DWORD-værdi **af EnableADAL** med en **indstilling på 0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="3a3ef-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="3a3ef-113">Du kan finde flere oplysninger under Problemer med forbindelse ved logon efter opdatering til [Office 2016 build 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="3a3ef-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>