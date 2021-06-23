---
title: Aktivér SMTP-godkendelse og -fejlfinding
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077645"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="da8f1-102">Aktivér SMTP-godkendelse og -fejlfinding</span><span class="sxs-lookup"><span data-stu-id="da8f1-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="da8f1-103">Hvis du vil aktivere SMTP-godkendelse for en postkasse, eller hvis du får fejlen "Klient ikke godkendt", "Godkendelse mislykkedes" eller "SmtpClientAuthentication" med kode 5.7.57 eller 5.7.3 eller 5.7.139, når du forsøger at videresende mails ved at godkende en enhed eller et program med Microsoft 365, skal du udføre disse tre handlinger for at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="da8f1-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="da8f1-104">Deaktiver [Azure-sikkerhedsstandardindstillingerne](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ved at slå **Aktivér sikkerhedsstandard til** **Nej.**</span><span class="sxs-lookup"><span data-stu-id="da8f1-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="da8f1-105">a.</span><span class="sxs-lookup"><span data-stu-id="da8f1-105">a.</span></span> <span data-ttu-id="da8f1-106">Log på Azure-portalen som sikkerhedsadministrator, betinget adgangsadministrator eller global administrator.</span><span class="sxs-lookup"><span data-stu-id="da8f1-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="da8f1-107">b.</span><span class="sxs-lookup"><span data-stu-id="da8f1-107">b.</span></span> <span data-ttu-id="da8f1-108">Gå til Azure Active Directory > **Egenskaber.**</span><span class="sxs-lookup"><span data-stu-id="da8f1-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="da8f1-109">c.</span><span class="sxs-lookup"><span data-stu-id="da8f1-109">c.</span></span> <span data-ttu-id="da8f1-110">Vælg **Administrer sikkerhedsstandardindstillinger.**</span><span class="sxs-lookup"><span data-stu-id="da8f1-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="da8f1-111">d.</span><span class="sxs-lookup"><span data-stu-id="da8f1-111">d.</span></span> <span data-ttu-id="da8f1-112">Angiv **Aktivér sikkerhedsstandard til** **Nej.**</span><span class="sxs-lookup"><span data-stu-id="da8f1-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="da8f1-113">e.</span><span class="sxs-lookup"><span data-stu-id="da8f1-113">e.</span></span> <span data-ttu-id="da8f1-114">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="da8f1-114">Select **Save**.</span></span>

2. <span data-ttu-id="da8f1-115">[Aktivér klient-SMTP-indsendelse](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) på den licenserede postkasse.</span><span class="sxs-lookup"><span data-stu-id="da8f1-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="da8f1-116">a.</span><span class="sxs-lookup"><span data-stu-id="da8f1-116">a.</span></span> <span data-ttu-id="da8f1-117">Fra Microsoft 365 Administration skal du gå **til Aktive** brugere og vælge brugeren.</span><span class="sxs-lookup"><span data-stu-id="da8f1-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="da8f1-118">b.</span><span class="sxs-lookup"><span data-stu-id="da8f1-118">b.</span></span> <span data-ttu-id="da8f1-119">Gå til fanen Mail, og vælg **Administrer mailapps** **under Mailapps**.</span><span class="sxs-lookup"><span data-stu-id="da8f1-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="da8f1-120">d.</span><span class="sxs-lookup"><span data-stu-id="da8f1-120">d.</span></span> <span data-ttu-id="da8f1-121">Kontrollér, **at Godkendt SMTP er** markeret (aktiveret).</span><span class="sxs-lookup"><span data-stu-id="da8f1-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="da8f1-122">e.</span><span class="sxs-lookup"><span data-stu-id="da8f1-122">e.</span></span> <span data-ttu-id="da8f1-123">Vælg **Gem ændringer**.</span><span class="sxs-lookup"><span data-stu-id="da8f1-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="da8f1-124">[Deaktiver Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) på den licenserede postkasse.</span><span class="sxs-lookup"><span data-stu-id="da8f1-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="da8f1-125">a.</span><span class="sxs-lookup"><span data-stu-id="da8f1-125">a.</span></span> <span data-ttu-id="da8f1-126">Gå til fanen Microsoft 365 Administration, og vælg Aktive brugere i **venstre navigationsmenu.**  >  </span><span class="sxs-lookup"><span data-stu-id="da8f1-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="da8f1-127">b.</span><span class="sxs-lookup"><span data-stu-id="da8f1-127">b.</span></span> <span data-ttu-id="da8f1-128">Vælg **Multifaktorgodkendelse.**</span><span class="sxs-lookup"><span data-stu-id="da8f1-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="da8f1-129">c.</span><span class="sxs-lookup"><span data-stu-id="da8f1-129">c.</span></span> <span data-ttu-id="da8f1-130">Vælg brugeren, og **deaktiver Multi-Factor Auth**.</span><span class="sxs-lookup"><span data-stu-id="da8f1-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
