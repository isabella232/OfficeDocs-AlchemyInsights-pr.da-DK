---
title: Fjern baggrundstjenesten til Microsoft Søg i Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816124"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="90d4a-102">Fjern baggrundstjenesten til Microsoft Søg i Bing</span><span class="sxs-lookup"><span data-stu-id="90d4a-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="90d4a-103">Hvis du vil fjerne baggrundstjenesten til Microsoft Søg i Bing, kan du prøve følgende afhjælpninger:</span><span class="sxs-lookup"><span data-stu-id="90d4a-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="90d4a-104">Hvis du vil vende tilbage til de oprindelige søgemaskineindstillinger, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="90d4a-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="90d4a-105">a.</span><span class="sxs-lookup"><span data-stu-id="90d4a-105">a.</span></span> <span data-ttu-id="90d4a-106">Slå **Brug Bing som din [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) standardsøgemaskine fra.**</span><span class="sxs-lookup"><span data-stu-id="90d4a-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="90d4a-107">b.</span><span class="sxs-lookup"><span data-stu-id="90d4a-107">b.</span></span> <span data-ttu-id="90d4a-108">[Gå til Microsoft 365 Administration, og](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ryd den indstilling, der påvirker alle brugere i organisationen.</span><span class="sxs-lookup"><span data-stu-id="90d4a-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="90d4a-109">Hvis du vil fjerne baggrundstjenesten fra en enkelt enhed, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="90d4a-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="90d4a-110">a.</span><span class="sxs-lookup"><span data-stu-id="90d4a-110">a.</span></span> <span data-ttu-id="90d4a-111">Vælg **Kontrolpanel > programmer > programmer og funktioner.**</span><span class="sxs-lookup"><span data-stu-id="90d4a-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="90d4a-112">b.</span><span class="sxs-lookup"><span data-stu-id="90d4a-112">b.</span></span> <span data-ttu-id="90d4a-113">Højreklik på **Microsoft Søg i Bing** under listen over installerede programmer, og klik derefter på **Fjern.**</span><span class="sxs-lookup"><span data-stu-id="90d4a-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="90d4a-114">Hvis du vil fjerne baggrundstjenesten fra flere enheder i organisationen, skal du logge på som administrator og køre følgende kommando i et script:</span><span class="sxs-lookup"><span data-stu-id="90d4a-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
