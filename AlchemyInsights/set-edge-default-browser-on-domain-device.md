---
title: Angiv Microsoft Edge som standardbrowser på en domæneforenet enhed
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491441"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="19790-102">Angiv Microsoft Edge som standardbrowser på en domæneforenet enhed</span><span class="sxs-lookup"><span data-stu-id="19790-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="19790-103">Angiv Microsoft Edge som standardbrowser:</span><span class="sxs-lookup"><span data-stu-id="19790-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="19790-104">[Opret en standardtilknytninger for](https://go.microsoft.com/fwlink/?linkid=2132437) konfigurationsfilen, og gem den lokalt eller på et netværksshare.</span><span class="sxs-lookup"><span data-stu-id="19790-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="19790-105">Åbn editoren Gruppepolitik, og gå derefter til Administrative skabeloner til  >  **computerkonfiguration,**  >  **Windows Components**  >  **Stifinder.**</span><span class="sxs-lookup"><span data-stu-id="19790-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="19790-106">Vælg **Angiv en standard tilknytninger til konfigurationsfil.**</span><span class="sxs-lookup"><span data-stu-id="19790-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="19790-107">Vælg **Politikindstilling,** og vælg derefter **Aktiveret.**</span><span class="sxs-lookup"><span data-stu-id="19790-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="19790-108">Under **Indstillinger** skal du angive placeringen af standard tilknytninger til konfigurationsfilen og derefter vælge **OK.**</span><span class="sxs-lookup"><span data-stu-id="19790-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
