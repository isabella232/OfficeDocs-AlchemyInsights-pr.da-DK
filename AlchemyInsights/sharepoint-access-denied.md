---
title: Foretag fejlfinding af meddelelser om nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691677"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="6c732-102">Foretag fejlfinding af meddelelser om nægtet adgang</span><span class="sxs-lookup"><span data-stu-id="6c732-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="6c732-103">Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gennemse et SharePoint Online-websted, skal du se nedenstående artikler.</span><span class="sxs-lookup"><span data-stu-id="6c732-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="6c732-104">**Tilføje og licensere brugeren**</span><span class="sxs-lookup"><span data-stu-id="6c732-104">**Add and License the user**</span></span>

<span data-ttu-id="6c732-105">Kontrollér, at du [tildeler licenser til brugere i Microsoft 365 til virksomheder](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="6c732-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="6c732-106">**Tildel tilladelser**</span><span class="sxs-lookup"><span data-stu-id="6c732-106">**Assign Permissions**</span></span>

<span data-ttu-id="6c732-107">Hvis brugeren har fået tildelt en SharePoint-licens, og du stadig modtager en meddelelse om adgang nægtet, skal du sørge for, at de har de [relevante tilladelsesniveauer tildelt](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="6c732-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="6c732-108">**Overvej at bruge funktionen anmodning om adgang**</span><span class="sxs-lookup"><span data-stu-id="6c732-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="6c732-109">[Adgangs anmodnings](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) funktionen gør det muligt for personer at anmode om adgang til indhold, som de ikke aktuelt har tilladelse til at se.</span><span class="sxs-lookup"><span data-stu-id="6c732-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="6c732-110">**Tillad, at brugerdefineret script muligvis får adgang til at nægte problemer**</span><span class="sxs-lookup"><span data-stu-id="6c732-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="6c732-111">Der er visse scenarier, hvor funktionen "Tillad brugerdefineret script" muligvis har adgang til at få adgang til at blive nægtet.</span><span class="sxs-lookup"><span data-stu-id="6c732-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="6c732-112">Hvis du vil have en liste over funktioner, der er påvirket, sikkerhedsovervejelser og muligheden for at deaktivere funktionen.</span><span class="sxs-lookup"><span data-stu-id="6c732-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="6c732-113">Besøg, [Tillad eller Forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="6c732-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="6c732-114">Bemærk! Hvis et OneDrive-eller SharePoint-websted ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt tjeneste problem.</span><span class="sxs-lookup"><span data-stu-id="6c732-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="6c732-115">[Se dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6c732-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

