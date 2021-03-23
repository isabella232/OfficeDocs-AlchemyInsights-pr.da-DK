---
title: Frier plads på drevet i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035665"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="6d798-102">Frier plads på drevet i Windows 10</span><span class="sxs-lookup"><span data-stu-id="6d798-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="6d798-103">Her er to muligheder for at frigøre plads på drevet i Windows:</span><span class="sxs-lookup"><span data-stu-id="6d798-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="6d798-104">Frier plads på drevet i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6d798-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="6d798-105">Frier plads til Windows 10-opdateringer med en ekstern lagerenhed.</span><span class="sxs-lookup"><span data-stu-id="6d798-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="6d798-106">Hvis du stadig har for lidt diskplads efter brug af Diskoprydning, er det muligt, at din Temp-mappe hurtigt bliver fyldt med programfiler (.appx), der bruges af Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="6d798-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="6d798-107">Du kan løse dette problem ved at nulstille Store, rydde Store-cachen og derefter køre Windows Update-fejlfindingsværktøjet.</span><span class="sxs-lookup"><span data-stu-id="6d798-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="6d798-108">Sørg for, at Microsoft Store er lukket, før du fortsætter med disse trin.</span><span class="sxs-lookup"><span data-stu-id="6d798-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="6d798-109">**Trin 1: Nulstil Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="6d798-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="6d798-110">**Bemærk!** Dette sletter appdataene på enheden permanent, herunder dine indstillinger og logonoplysninger.</span><span class="sxs-lookup"><span data-stu-id="6d798-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="6d798-111">Vælg **Start indstillinger**  >  **for**  >  **apps** og &  >  **funktioner.**</span><span class="sxs-lookup"><span data-stu-id="6d798-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="6d798-112">Find og vælg Microsoft Store på listen over apps.</span><span class="sxs-lookup"><span data-stu-id="6d798-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="6d798-113">Vælg **Avancerede indstillinger.**</span><span class="sxs-lookup"><span data-stu-id="6d798-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="6d798-114">Rul ned, vælg **Nulstil,** og **bekræft derefter nulstilling.**</span><span class="sxs-lookup"><span data-stu-id="6d798-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="6d798-115">**Trin 2: Ryd Microsoft Store-cachen**</span><span class="sxs-lookup"><span data-stu-id="6d798-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="6d798-116">Tryk på Windows-tasten + R for at åbne dialogboksen Kør.</span><span class="sxs-lookup"><span data-stu-id="6d798-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="6d798-117">Skriv wsreset.exe, og vælg **OK.**</span><span class="sxs-lookup"><span data-stu-id="6d798-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="6d798-118">Der åbnes et tomt kommandopromptvindue.</span><span class="sxs-lookup"><span data-stu-id="6d798-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="6d798-119">Efter ca. 10 sekunder lukkes vinduet, og Store åbnes automatisk.</span><span class="sxs-lookup"><span data-stu-id="6d798-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="6d798-120">**Trin 3: Nulstil Windows Update**</span><span class="sxs-lookup"><span data-stu-id="6d798-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="6d798-121">Vælg **Opdatering af**  >    >  **startindstillinger & Sikkerhedsfejlfinding.**  >  </span><span class="sxs-lookup"><span data-stu-id="6d798-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="6d798-122">Rul ned, **og vælg Windows Update** på listen, og vælg Kør **fejlfindingsværktøjet.**</span><span class="sxs-lookup"><span data-stu-id="6d798-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="6d798-123">Genstart computeren, og kontrollér, om du stadig oplever problemet.</span><span class="sxs-lookup"><span data-stu-id="6d798-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

