---
title: Oplåsning af en konto
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
- "9002449"
- "4748"
ms.openlocfilehash: 532b273154a31c024825b150d9b0edd42eb6130c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827750"
---
# <a name="unlocking-an-account"></a><span data-ttu-id="ad8ce-102">Oplåsning af en konto</span><span class="sxs-lookup"><span data-stu-id="ad8ce-102">Unlocking an account</span></span>

<span data-ttu-id="ad8ce-103">Det kan ske, at brugere låses ude af Microsoft 365 pga. for mange forkerte adgangskodeforsøg eller andre problemer.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-103">It's possible users are locked out of Microsoft 365 due to bad password attempts or other compromises.</span></span> <span data-ttu-id="ad8ce-104">For at hjælpe brugerne med at logge på Microsoft 365 igen **kan du prøve følgende trin, inden du åbner en supportanmodning**.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-104">To help users sign back in to Microsoft 365, **you can attempt the following steps before opening a Support Request**.</span></span> 

<span data-ttu-id="ad8ce-105">**Begrænset mail**</span><span class="sxs-lookup"><span data-stu-id="ad8ce-105">**Email Restricted**</span></span>

<span data-ttu-id="ad8ce-106">Hvis en af brugerne er begrænset fra at sende en mail, kan du som administrator [fjerne blokeringen af kontoen selv](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span><span class="sxs-lookup"><span data-stu-id="ad8ce-106">As an admin, if one of your users is restricted from sending email, you can [unblock the account yourself](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span></span> <span data-ttu-id="ad8ce-107">Brugeren kan sende mails inden for en time, efter du har fjernet begrænsningen.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-107">The user will be able to send email within an hour after removing the restriction.</span></span>

<span data-ttu-id="ad8ce-108">**Nulstil brugerens adgangskode**</span><span class="sxs-lookup"><span data-stu-id="ad8ce-108">**Reset the User Password**</span></span>

1. <span data-ttu-id="ad8ce-109">I Administration gå til **Brugere > [Aktive brugere](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-109">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="ad8ce-110">Vælg brugeren, og klik på **Nulstil adgangskode**.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-110">Select the user and click **Reset Password**.</span></span>

<span data-ttu-id="ad8ce-111">**Kontrollér, at brugeren har tilladelse til at logge på**</span><span class="sxs-lookup"><span data-stu-id="ad8ce-111">**Make sure the user is allowed to sign in**</span></span>

1. <span data-ttu-id="ad8ce-112">I Administration gå til **Brugere > [Aktive brugere](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-112">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="ad8ce-113">Vælg brugeren, og klik på **Flere handlinger (...)**, og klik derefter på **Rediger status for logon**.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-113">Select the user and click **More Actions (...)**; then click **Edit sign-in status**.</span></span>

<span data-ttu-id="ad8ce-114">Hvis du vil se flere scenarier til nulstilling af adgangskode, herunder selvbetjening til nulstilling af adgangskode, skal du se [Nulstil adgangskoder til Microsoft 365 til virksomheder](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ad8ce-114">For more password reset scenarios, including Self-Service Password Reset, see [Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords?view=o365-worldwide).</span></span>

<span data-ttu-id="ad8ce-115">Tjenesten forhindrer, at en bruger kan sende mails efter at have påvist dokumentation for en kompromitteret konto og/eller udgående spam.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-115">The service prevents a user from sending email after detecting evidence of a compromised account and/or outbound spam.</span></span> <span data-ttu-id="ad8ce-116">Som forholdsregel skal du følge trinnene for [reaktion på en kompromitteret mailkonto i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) for brugeren.</span><span class="sxs-lookup"><span data-stu-id="ad8ce-116">As a precaution, follow the steps in [Responding to a Compromised Email Account in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) for the user.</span></span>
