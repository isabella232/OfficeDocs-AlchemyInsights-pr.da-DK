---
title: Identificer ekstern videresendelse af mail i postkasser i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508946"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="f8ce2-102">Identificer, hvornår ekstern videresendelse af mail er konfigureret i postkasser</span><span class="sxs-lookup"><span data-stu-id="f8ce2-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="f8ce2-103">Når en Microsoft 365-bruger konfigurerer ekstern videresendelse af mail i en postkasse, overvåges aktiviteten som en del af **cmdlet'en set-postkasse.**</span><span class="sxs-lookup"><span data-stu-id="f8ce2-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="f8ce2-104">Du kan se aktiviteten ved hjælp af søgning i overvågningsloggen i Sikkerheds- & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="f8ce2-105">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f8ce2-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f8ce2-106">Gå til søgesiden for søgesøgning i søgeloggen søge i søgeloggen **for søgeloggen søge**i søgeloggen for  >  **søgesøgning.**</span><span class="sxs-lookup"><span data-stu-id="f8ce2-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="f8ce2-107">Vælg datointervallet i felterne **Startdato** og **Slutdato.**</span><span class="sxs-lookup"><span data-stu-id="f8ce2-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="f8ce2-108">Du behøver ikke at angive et brugernavn.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-108">You don't need to specify a username.</span></span> <span data-ttu-id="f8ce2-109">Kontroller, at feltet **Aktiviteter** er angivet til **Vis resultater for alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="f8ce2-110">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-110">Click **Search**.</span></span>

<span data-ttu-id="f8ce2-111">Klik på **Filtrer resultater** i resultaterne, og skriv **Angiv postkasse** i aktivitetsfilterfeltet.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="f8ce2-112">Vælg en overvågningspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-112">Select an audit record in the results.</span></span> <span data-ttu-id="f8ce2-113">Klik på **Flere oplysninger**i pop op-vinduet **Detaljer** .</span><span class="sxs-lookup"><span data-stu-id="f8ce2-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="f8ce2-114">Du skal se på detaljerne i hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af e-mail.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="f8ce2-115">**ObjectId**: Aliasværdien for den postkasse, der blev ændret.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="f8ce2-116">**Parametre**: _ForwardingSmtpAddress_ angiver destinations-e-mailadressen.</span><span class="sxs-lookup"><span data-stu-id="f8ce2-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="f8ce2-117">**UserId**: Den bruger, der har konfigureret videresendelse af mail på postkassen i feltet **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="f8ce2-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="f8ce2-118">Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail til en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="f8ce2-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
