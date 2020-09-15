---
title: DTT til SharePoint, OneDrive og Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715555"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="7ae24-102">DTT til SharePoint, OneDrive og Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="7ae24-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="7ae24-103">Følg disse trin for at aktivere avanceret trusselsbeskyttelse:</span><span class="sxs-lookup"><span data-stu-id="7ae24-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="7ae24-104">Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator-eller sikkerhedsadministrator konto.</span><span class="sxs-lookup"><span data-stu-id="7ae24-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="7ae24-105">Vælg **politik** sikre vedhæftede filer i venstre navigationsrude under **trussels administration** \> **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="7ae24-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="7ae24-106">Vælg **Aktivér DTT for SharePoint, OneDrive og Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="7ae24-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="7ae24-107">[Opret en politik for besked om aktivitet](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for at modtage meddelelser, når vi registrerer ondsindede filer.</span><span class="sxs-lookup"><span data-stu-id="7ae24-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="7ae24-108">Du kan finde en komplet vejledning i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="7ae24-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="7ae24-109">**Bemærk**: efter design scanner DTT ikke alle enkeltfiler i SharePoint Online, OneDrive for Business eller Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="7ae24-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="7ae24-110">Filer scannes asynkront af en proces, der bruger delings aktivitet, gæste aktivitet og trusler signaler til at identificere ondsindede filer.</span><span class="sxs-lookup"><span data-stu-id="7ae24-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="7ae24-111">Du kan finde flere oplysninger i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="7ae24-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
