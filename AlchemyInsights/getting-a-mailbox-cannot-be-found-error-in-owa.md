---
title: 126 hentning af en postkasse kan ikke finde fejlen i OWA?
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
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706744"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="4fe80-102">Kan du ikke finde fejlen i postkassen i Outlook på internettet?</span><span class="sxs-lookup"><span data-stu-id="4fe80-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="4fe80-103">Hvis du bruger Outlook på internettet, og du får en postkasse, der ikke **blev fundet for** fejlen, har den konto, du brugte til at oprette forbindelse til Outlook på internettet, ikke en Exchange Online-licens, og der er derfor ikke knyttet nogen postkasse til kontoen.</span><span class="sxs-lookup"><span data-stu-id="4fe80-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="4fe80-104">Din administrator kan tildele en licens til din konto ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="4fe80-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="4fe80-105">Åbn [Microsoft 365 administration](https://portal.office.com/adminportal/home#/homepage) , og gå til **aktive brugere** under sektionen **brugere** , og vælg den bruger, der får vist fejlen.</span><span class="sxs-lookup"><span data-stu-id="4fe80-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="4fe80-106">På den bruger side, der åbnes, skal du gå til sektionen **licenser og apps** , vælge den relevante **placerings** værdi og tildele en licens, der indeholder Exchange Online (Udvid licensen for at se dens detaljer).</span><span class="sxs-lookup"><span data-stu-id="4fe80-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="4fe80-107">Når du er færdig, skal du klikke på **Gem ændringer**.</span><span class="sxs-lookup"><span data-stu-id="4fe80-107">When you're finished, click **Save changes**.</span></span>
