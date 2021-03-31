---
title: 126 Fejlen "Henter en postkasse" i OWA blev ikke fundet?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426656"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="bbde7-102">Får du en postkassefejl, som ikke blev fundet i Outlook på internettet?</span><span class="sxs-lookup"><span data-stu-id="bbde7-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="bbde7-103">Hvis du bruger Outlook på internettet, og du får en postkasse, der ikke blev fundet **som** fejl, har den konto, du brugte til at oprette forbindelse til Outlook på internettet, ikke en Exchange Online-licens, og derfor er der ikke knyttet nogen postkasse til kontoen.</span><span class="sxs-lookup"><span data-stu-id="bbde7-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="bbde7-104">Din administrator kan tildele en licens til din konto ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="bbde7-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="bbde7-105">Åbn [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) Administration, og gå  til **Aktive** brugere under sektionen Brugere, og vælg den bruger, der får vist fejlen.</span><span class="sxs-lookup"><span data-stu-id="bbde7-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="bbde7-106">På brugersiden, der åbnes, skal du gå til  sektionen Licenser og **apps,** vælge den relevante placeringsværdi og tildele en licens, der indeholder Exchange Online (udvid licensen for at få vist dens detaljer).</span><span class="sxs-lookup"><span data-stu-id="bbde7-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="bbde7-107">Klik på Gem ændringer, når du **er færdig.**</span><span class="sxs-lookup"><span data-stu-id="bbde7-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="bbde7-108">I nogle tilfælde, hvis licensen allerede er tildelt en brugerkonto, hjælper fjernelse og gentildeling af licensen med at løse problemet og få den klargjort korrekt i systemet:</span><span class="sxs-lookup"><span data-stu-id="bbde7-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="bbde7-109">Kontrollér, om dine M365 Exchange Online-abonnementer (og andre, hvis du har nogen) er aktuelle og ikke er udløbet for nylig.</span><span class="sxs-lookup"><span data-stu-id="bbde7-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="bbde7-110">Når du har kontrolleret, at dit abonnement ikke er udløbet, og der er tildelt en gyldig licens til brugerkontoen, kan der gå op til 24 timer, før licensen er klargjort, så det kan være en god ide at vente på, at problemet bliver løst.</span><span class="sxs-lookup"><span data-stu-id="bbde7-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="bbde7-111">Du kan få mere at vide [under Tildel og administrer licenser.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="bbde7-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>