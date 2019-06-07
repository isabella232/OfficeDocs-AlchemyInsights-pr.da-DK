---
title: DTT for SharePoint, OneDrive og Microsoft-Team
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764948"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="31dee-102">DTT for SharePoint, OneDrive og Microsoft-Team</span><span class="sxs-lookup"><span data-stu-id="31dee-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="31dee-103">Følg disse trin for at aktivere avanceret Threat Protection:</span><span class="sxs-lookup"><span data-stu-id="31dee-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="31dee-104">Gå til [https://protection.office.com](https://protection.office.com) og logge på med en global administrator eller sikkerhedsadministratorkonto.</span><span class="sxs-lookup"><span data-stu-id="31dee-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="31dee-105">Vælg **politik** i den venstre navigationsrude under **Administration af truslen**, \> **Sikre vedhæftede filer**.</span><span class="sxs-lookup"><span data-stu-id="31dee-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="31dee-106">Vælg **Slå DTT for SharePoint, OneDrive, og Microsoft-Team**.</span><span class="sxs-lookup"><span data-stu-id="31dee-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="31dee-107">[Oprette en aktivitet besked politik](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) til at modtage besked, når vi registrere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="31dee-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="31dee-108">Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="31dee-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="31dee-109">**Bemærk**: ved design, ATP ikke scanne hver enkelt fil i SharePoint Online, OneDrive til arbejde eller Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="31dee-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="31dee-110">Filer scannes asynkront ved en proces, der bruger Deling aktivitet, aktivitet for gæst, og truslen signaler til at identificere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="31dee-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="31dee-111">Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="31dee-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
