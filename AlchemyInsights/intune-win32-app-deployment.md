---
title: Installation af Win32-app til Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461759"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="dfd68-102">Installation af Win32-app til Win32</span><span class="sxs-lookup"><span data-stu-id="dfd68-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="dfd68-103">Microsoft Intune tillader Win32-programmer, herunder, men ikke begrænset til MSI og. EXE skal installeres på Windows 10-enheder.</span><span class="sxs-lookup"><span data-stu-id="dfd68-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="dfd68-104">Den anvendte installationsmekanisme kræver, at Intune Management Extension er tilgængelig på destinationsenheden.</span><span class="sxs-lookup"><span data-stu-id="dfd68-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="dfd68-105">IME installeres automatisk som et resultat af målretning af et PowerShell-script eller en Win32-Programinstallation til en bruger/enhed.</span><span class="sxs-lookup"><span data-stu-id="dfd68-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="dfd68-106">Der er også en række forudsætninger, der skal opfyldes, for at du kan installere Win32-apps, der omfatter:</span><span class="sxs-lookup"><span data-stu-id="dfd68-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="dfd68-107">Understøttede platforme: Windows 10 version 1607 eller nyere (Enterprise, Pro og Education versions).</span><span class="sxs-lookup"><span data-stu-id="dfd68-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="dfd68-108">Understøttet arkitektur: x86 og x64.</span><span class="sxs-lookup"><span data-stu-id="dfd68-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="dfd68-109">Enhedshåndtering: AAD-tilmeldt og automatisk tilmeldt (herunder hybridt domæne, der er joinforbundet og Gruppepolitik automatisk tilmeldt).</span><span class="sxs-lookup"><span data-stu-id="dfd68-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="dfd68-110">Programpakke format:. **intunewin**  -fil, der er udarbejdet af [Microsoft Win32-indholds forberedelsesværktøjet](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="dfd68-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="dfd68-111">Begrænsede</span><span class="sxs-lookup"><span data-stu-id="dfd68-111">Limitations:</span></span>
    - <span data-ttu-id="dfd68-112">Maksimal størrelse: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="dfd68-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="dfd68-113">Ikke-understøttet arkitektur: arme.</span><span class="sxs-lookup"><span data-stu-id="dfd68-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="dfd68-114">Gennemse dokumentet "[Tilføj, Tildel og Overvåg en Win32-app i Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for oplysninger, der er relateret til disse trin.</span><span class="sxs-lookup"><span data-stu-id="dfd68-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="dfd68-115">Oplysninger om fejlfinding i forbindelse med installation af programmer på Windows, herunder Win32-apps, kan gennemses i følgende dokumenter</span><span class="sxs-lookup"><span data-stu-id="dfd68-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="dfd68-116">Fejlfinding af problemer med App-installation</span><span class="sxs-lookup"><span data-stu-id="dfd68-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="dfd68-117">Fejlfinding af Win32-apps</span><span class="sxs-lookup"><span data-stu-id="dfd68-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)