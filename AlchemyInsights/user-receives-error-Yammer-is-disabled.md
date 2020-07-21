---
title: Brugeren får vist fejl AADSTS7000112 Yammer er deaktiveret
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197874"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="07ec3-102">Brugeren får vist fejl AADSTS7000112 Yammer er deaktiveret</span><span class="sxs-lookup"><span data-stu-id="07ec3-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="07ec3-103">Hvis du får vist fejlmeddelelsen "AADSTS7000112: Programmet '00000005-0000-0ff1-ce00-0000000000'(Yammer) er deaktiveret", er der et problem med tjenesteproektoren i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="07ec3-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="07ec3-104">En administrator har muligvis deaktiveret tjenesterektoren for at blokere adgangen til Yammer.</span><span class="sxs-lookup"><span data-stu-id="07ec3-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="07ec3-105">Deaktivering af tjenesterektoren anbefales ikke og kan forårsage yderligere problemer.</span><span class="sxs-lookup"><span data-stu-id="07ec3-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="07ec3-106">Du kan finde flere oplysninger om den understøttede fremgangsmåde til at blokere brugeradgang til Yammer under [Slå Yammer-adgang fra for Microsoft 365-brugere](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="07ec3-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="07ec3-107">Sådan løser du dette problem på Azure Portal og gendanner brugeradgang til Yammer:</span><span class="sxs-lookup"><span data-stu-id="07ec3-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="07ec3-108">Åbn Siden Azure Active Directory, og vælg **Virksomhedsprogrammer** under **Administrer** i venstre navigationsrude.</span><span class="sxs-lookup"><span data-stu-id="07ec3-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="07ec3-109">Skriv **Office 365 Yammer** i søgefeltet, og vælg det programnavn, der skal åbnes indstillinger.</span><span class="sxs-lookup"><span data-stu-id="07ec3-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="07ec3-110">Vælg **Egenskaber** under **Administrer** i venstre navigationsrude.</span><span class="sxs-lookup"><span data-stu-id="07ec3-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="07ec3-111">Skal værdien **Aktiveret for brugere skal logge på til** **Ja**, og vælg derefter **Gem**.</span><span class="sxs-lookup"><span data-stu-id="07ec3-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="07ec3-112">Log på Yammer igen.</span><span class="sxs-lookup"><span data-stu-id="07ec3-112">Sign in to Yammer again.</span></span> <span data-ttu-id="07ec3-113">Du skal muligvis rydde cookies.</span><span class="sxs-lookup"><span data-stu-id="07ec3-113">You might need to clear cookies.</span></span>

<span data-ttu-id="07ec3-114">Du kan også køre PowerShell-kommandoer for at angive værdien.</span><span class="sxs-lookup"><span data-stu-id="07ec3-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="07ec3-115">Du kan finde flere oplysninger under [fejlen "Beklager, men vi har problemer med at logge dig på", når du klikker på Yammer-feltet i Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="07ec3-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 