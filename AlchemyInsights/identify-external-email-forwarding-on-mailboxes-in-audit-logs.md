---
title: Identificere ekstern videresendelse af mail på postkasser i overvågningslogfiler
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
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716454"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="7ab19-102">Identificer, hvornår ekstern videresendelse af mail er konfigureret i postkasser</span><span class="sxs-lookup"><span data-stu-id="7ab19-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="7ab19-103">Når en Microsoft 365-bruger konfigurerer ekstern videresendelse af mail på en postkasse, overvåges aktiviteten som en del af **cmdlet'en Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="7ab19-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="7ab19-104">Du kan se aktiviteten ved hjælp af overvågningslogsøgning i Sikkerheds& Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="7ab19-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="7ab19-105">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="7ab19-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="7ab19-106">Gå til**søgesiden for søgefilen til søgeovervågning** i **søgefilen** > til søgning i søgeområdet.</span><span class="sxs-lookup"><span data-stu-id="7ab19-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="7ab19-107">Vælg datointervallet i felterne **Startdato** **og Slutdato.**</span><span class="sxs-lookup"><span data-stu-id="7ab19-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="7ab19-108">Du behøver ikke at angive et brugernavn.</span><span class="sxs-lookup"><span data-stu-id="7ab19-108">You don't need to specify a username.</span></span> <span data-ttu-id="7ab19-109">Kontroller, at feltet **Aktiviteter** er angivet til Vis resultater for **alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="7ab19-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="7ab19-110">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="7ab19-110">Click **Search**.</span></span>

<span data-ttu-id="7ab19-111">Klik på **Filtrer resultater** i resultaterne, og skriv **Set-Postkasse** i feltet aktivitetsfilter.</span><span class="sxs-lookup"><span data-stu-id="7ab19-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="7ab19-112">Vælg en overvågningspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="7ab19-112">Select an audit record in the results.</span></span> <span data-ttu-id="7ab19-113">Klik på Flere oplysninger i pop **op-vinduet** **Detaljer** .</span><span class="sxs-lookup"><span data-stu-id="7ab19-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="7ab19-114">Du skal se på detaljerne for hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af e-mail.</span><span class="sxs-lookup"><span data-stu-id="7ab19-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="7ab19-115">**ObjectId**: Aliasværdien for den postkasse, der blev ændret.</span><span class="sxs-lookup"><span data-stu-id="7ab19-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="7ab19-116">**Parametre**: _Videresendelse SmtpAddress_ angiver destinationsmailadressen.</span><span class="sxs-lookup"><span data-stu-id="7ab19-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="7ab19-117">**UserId**: Den bruger, der konfigurerede videresendelse af mail på postkassen i **feltet ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="7ab19-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="7ab19-118">Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail for en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="7ab19-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
