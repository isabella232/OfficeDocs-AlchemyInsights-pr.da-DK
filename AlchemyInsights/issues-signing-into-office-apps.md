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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695173"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="b9e59-102">Rettelse af Microsoft 365-apps "din computers Trusted Platform-modul fungerer ikke korrekt"-meddelelse</span><span class="sxs-lookup"><span data-stu-id="b9e59-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="b9e59-103">Du kan rette fejlen ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="b9e59-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b9e59-104">Installer de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="b9e59-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b9e59-105">[Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows credential Manager.</span><span class="sxs-lookup"><span data-stu-id="b9e59-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b9e59-106">**Bemærk:** Registreringsdatabase stierne til Office 2016 er blevet ændret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="b9e59-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b9e59-107">(F. eks.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b9e59-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b9e59-108">Prøv [genoprettelsesprocessen for brugeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for at løse TPM-fejl (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="b9e59-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="b9e59-109">Angiv EnableADAL = 0 ved hjælp af følgende trin:</span><span class="sxs-lookup"><span data-stu-id="b9e59-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="b9e59-110">Højreklik på knappen Start i Windows, Vælg **Kør**, Skriv **regedit**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="b9e59-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="b9e59-111">Vælg **Ja** for at tillade, at registrerings Editor foretager ændringer på din enhed.</span><span class="sxs-lookup"><span data-stu-id="b9e59-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="b9e59-112">I registrerings Editor skal du tilføje en DWORD-værdi for **EnableADAL** med en indstilling på **0** under HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="b9e59-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="b9e59-113">Hvis du vil have mere at vide, skal du se [forbindelsesproblemer i logon efter opdatering til Office 2016 Build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="b9e59-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>