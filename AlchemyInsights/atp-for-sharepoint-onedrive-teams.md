---
title: ATP til SharePoint, OneDrive og Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712452"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="3b3a0-102">ATP til SharePoint, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3b3a0-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="3b3a0-103">Følg disse trin for at aktivere Avanceret trusselsbeskyttelse:</span><span class="sxs-lookup"><span data-stu-id="3b3a0-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="3b3a0-104">Gå [https://protection.office.com](https://protection.office.com) til og log på med en global administrator- eller sikkerhedsadministratorkonto.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="3b3a0-105">Vælg **Politiksikre** \> vedhæftede filer i venstre navigationsrude under **Trusselsstyring**. **Safe Attachments**</span><span class="sxs-lookup"><span data-stu-id="3b3a0-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="3b3a0-106">Vælg **Slå ATP til for SharePoint, OneDrive og Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="3b3a0-107">[Opret en politik](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) for aktivitetsadvarsler for at modtage meddelelser, når vi registrerer skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="3b3a0-108">Du kan finde komplette instruktioner i dette [emne](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3b3a0-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="3b3a0-109">**Bemærk:** Efter design scanner ATP ikke hver eneste fil i SharePoint Online, OneDrive for Business eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="3b3a0-110">Filer scannes asynkront af en proces, der bruger delingsaktivitet, gæsteaktivitet og trusselssignaler til at identificere ondsindede filer.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="3b3a0-111">Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3b3a0-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
