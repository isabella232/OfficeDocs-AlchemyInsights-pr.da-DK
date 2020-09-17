---
title: Der kan ikke logges på teams på grund af fejl autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799954"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="f73e6-102">Det er ikke muligt at logge på teams på grund af fejl i automatisk logon. microsoftazuread-SSO-dk-com: 443</span><span class="sxs-lookup"><span data-stu-id="f73e6-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="f73e6-103">Hvis problemfrit SSO er aktiveret som O365-godkendelse, skal URL-adressen "autologon.microsoftazuread-sso.com" muligvis føjes til intranet websteder.</span><span class="sxs-lookup"><span data-stu-id="f73e6-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="f73e6-104">Hvis det tidligere er blevet føjet til websteder, der er tillid til, og problem løse SSO er i brug, bør det fjernes fra websteder, du har tillid til.</span><span class="sxs-lookup"><span data-stu-id="f73e6-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="f73e6-105">Gennemse [checklisten Problemløser for SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="f73e6-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="f73e6-106">Følg disse trin for at tilføje en URL-adresse på listen over intranet websteder:</span><span class="sxs-lookup"><span data-stu-id="f73e6-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="f73e6-107">Åbn Internet Explorer ved at klikke på knappen **Start** .</span><span class="sxs-lookup"><span data-stu-id="f73e6-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="f73e6-108">I søgefeltet skal du skrive Internet Explorer og derefter klikke på **Internet Explorer**på listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="f73e6-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="f73e6-109">Klik på **værktøjer**, og klik derefter på **Internet indstillinger**.</span><span class="sxs-lookup"><span data-stu-id="f73e6-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="f73e6-110">Klik på fanen **sikkerhed** .</span><span class="sxs-lookup"><span data-stu-id="f73e6-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="f73e6-111">Klik nu på **lokale intranet websteder** , og klik derefter på knappen **websteder** og derefter knappen **Avanceret** .</span><span class="sxs-lookup"><span data-stu-id="f73e6-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="f73e6-112">Indtast webstedets URL-adresse, og klik på **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="f73e6-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="f73e6-113">Klik på **Luk**, når du er færdig.</span><span class="sxs-lookup"><span data-stu-id="f73e6-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="f73e6-114">Du kan finde flere oplysninger i [dokumentationen til installation af problemfrit SSO til O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (omfatter politikbaseret proces, hvor du kan tilføje en URL-adresse til intranet websteder i trin 3).</span><span class="sxs-lookup"><span data-stu-id="f73e6-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
