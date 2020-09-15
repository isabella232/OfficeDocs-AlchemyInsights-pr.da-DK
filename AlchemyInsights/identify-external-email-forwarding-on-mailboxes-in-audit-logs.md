---
title: Identificer ekstern videresendelse af mail i postkasser i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696291"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="b03d7-102">Identificer, hvornår videresendelse af ekstern mail er konfigureret på postkasser</span><span class="sxs-lookup"><span data-stu-id="b03d7-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="b03d7-103">Når en Microsoft 365-bruger konfigurerer ekstern videresendelse af mail i en postkasse, overvåges aktiviteten som en del af cmdlet'en **set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="b03d7-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="b03d7-104">Du kan se aktiviteten ved hjælp af søgning i overvågningsloggen i sikkerheds & overholdelses Center.</span><span class="sxs-lookup"><span data-stu-id="b03d7-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="b03d7-105">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="b03d7-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="b03d7-106">Gå til søgesiden **Søg i**  >  **overvågningslogfil** .</span><span class="sxs-lookup"><span data-stu-id="b03d7-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="b03d7-107">Vælg datointervallet i felterne **Start dato** og **Slutdato** .</span><span class="sxs-lookup"><span data-stu-id="b03d7-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="b03d7-108">Du behøver ikke at angive et Brugernavn.</span><span class="sxs-lookup"><span data-stu-id="b03d7-108">You don't need to specify a username.</span></span> <span data-ttu-id="b03d7-109">Kontrollér, at feltet **aktiviteter** er indstillet til at **vise resultater for alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="b03d7-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="b03d7-110">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="b03d7-110">Click **Search**.</span></span>

<span data-ttu-id="b03d7-111">I resultaterne skal du klikke på **filter resultater** og skrive **set-postkasse** i feltet aktivitets filter.</span><span class="sxs-lookup"><span data-stu-id="b03d7-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="b03d7-112">Vælg en revisionspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="b03d7-112">Select an audit record in the results.</span></span> <span data-ttu-id="b03d7-113">Klik på **flere oplysninger**i pop op-vinduet **detaljer** .</span><span class="sxs-lookup"><span data-stu-id="b03d7-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="b03d7-114">Du skal se nærmere på detaljerne for hver revisionspost for at afgøre, om aktiviteten er relateret til videresendelse af mail.</span><span class="sxs-lookup"><span data-stu-id="b03d7-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="b03d7-115">**ObjectId**: alias værdien for den postkasse, der blev ændret.</span><span class="sxs-lookup"><span data-stu-id="b03d7-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="b03d7-116">**Parametre**: _ForwardingSmtpAddress_ Angiver destinations mailadressen.</span><span class="sxs-lookup"><span data-stu-id="b03d7-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="b03d7-117">**UserID**: den bruger, der har konfigureret videresendelse af mails, i feltet ObjectId i feltet **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="b03d7-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="b03d7-118">Hvis du vil have mere at vide, skal du se [bestemme, hvem der skal konfigurere videresendelse af mail for en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)</span><span class="sxs-lookup"><span data-stu-id="b03d7-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
