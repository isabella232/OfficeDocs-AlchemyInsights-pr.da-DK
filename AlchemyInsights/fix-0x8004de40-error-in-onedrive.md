---
title: Ret 0x8004de40 fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649742"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="69542-102">Ret 0x8004de40 fejl i OneDrive</span><span class="sxs-lookup"><span data-stu-id="69542-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="69542-103">Hvis du kører Windows 7 og modtager denne fejl, skal du opdatere for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows.</span><span class="sxs-lookup"><span data-stu-id="69542-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="69542-104">Hvis du kører Windows 10, og du modtager en fejlmeddelelse 0x8004de40 med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="69542-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="69542-105">Genstart den påvirkede computer, mens du har forbindelse til dit Acitve-mappedomæne.</span><span class="sxs-lookup"><span data-stu-id="69542-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="69542-106">Hvis en genstart ikke løser problemet, skal du fjerne forbindelse til og slutte enheden til din enhed igen fra Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69542-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="69542-107">**Bemærk!** Du bør være på virksomhedens netværk, mens du udfører disse trin.</span><span class="sxs-lookup"><span data-stu-id="69542-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="69542-108">Udfør ikke disse trin, når du ikke har forbindelse til virksomhedens infrastruktur (f.eks. mens du rejser).</span><span class="sxs-lookup"><span data-stu-id="69542-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="69542-109">Åbn en kommandoprompt med administratorrettigheder ved at vælge **Start**, højreklik **på Kommandoprompt**, og vælg **derefter Kør som administrator**.</span><span class="sxs-lookup"><span data-stu-id="69542-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="69542-110">Skriv *dsregcmd /leave, og* tryk på **Enter.**</span><span class="sxs-lookup"><span data-stu-id="69542-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="69542-111">Når du er færdig, skal *du skrive dsregcmd /join* og trykke på **Enter.**</span><span class="sxs-lookup"><span data-stu-id="69542-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="69542-112">Luk kommandoprompten, når du er færdig.</span><span class="sxs-lookup"><span data-stu-id="69542-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="69542-113">Genstart computeren, og log på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="69542-113">Reboot the computer, and log into OneDrive.</span></span>