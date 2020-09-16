---
title: Problemer med ydeevnen – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771238"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="742ce-102">SharePoint eller OneDrive langsom, utilgængelig eller ikke tilgængelig for flere brugere</span><span class="sxs-lookup"><span data-stu-id="742ce-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="742ce-103">Hvis et OneDrive-eller SharePoint-websted ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt tjeneste problem.</span><span class="sxs-lookup"><span data-stu-id="742ce-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="742ce-104">[Se dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="742ce-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="742ce-105">**Tilføje og licensere brugeren**</span><span class="sxs-lookup"><span data-stu-id="742ce-105">**Add and license the user**</span></span>

<span data-ttu-id="742ce-106">Kontrollér, at du [tildeler licenser til brugere i Microsoft 365 til virksomheder](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="742ce-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="742ce-107">**Tildel tilladelser**</span><span class="sxs-lookup"><span data-stu-id="742ce-107">**Assign Permissions**</span></span>

<span data-ttu-id="742ce-108">Hvis brugeren har fået tildelt en SharePoint-licens, og du stadig modtager en meddelelse om adgang nægtet, skal du sørge for, at de har de [relevante tilladelsesniveauer](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tildelt.</span><span class="sxs-lookup"><span data-stu-id="742ce-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="742ce-109">**Overvej at bruge funktionen anmodning om adgang**</span><span class="sxs-lookup"><span data-stu-id="742ce-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="742ce-110">[Adgangs anmodnings funktionen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) gør det muligt for personer at anmode om adgang til indhold, som de ikke aktuelt har tilladelse til at se.</span><span class="sxs-lookup"><span data-stu-id="742ce-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="742ce-111">**Tillad, at brugerdefineret script muligvis får adgang til at nægte problemer**</span><span class="sxs-lookup"><span data-stu-id="742ce-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="742ce-112">Der er visse scenarier, hvor funktionen til *at aktivere brugerdefinerede scripts* muligvis har en adgang, der er nægtet.</span><span class="sxs-lookup"><span data-stu-id="742ce-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="742ce-113">Hvis du vil have en liste over funktioner, der er påvirket, sikkerhedsovervejelser og muligheden for at deaktivere funktionen.</span><span class="sxs-lookup"><span data-stu-id="742ce-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="742ce-114">Gå til [Tillad eller Forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="742ce-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

