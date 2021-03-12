---
title: Ret indstillinger for brugerpolitik/postkasse
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744840"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="4c92e-102">Ret indstillinger for brugerpolitik/postkasse</span><span class="sxs-lookup"><span data-stu-id="4c92e-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="4c92e-103">Indstillingerne for uønsket mail på postkassen påvirkede denne meddelelse.</span><span class="sxs-lookup"><span data-stu-id="4c92e-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="4c92e-104">Hvis du vil gennemse indstillingerne, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="4c92e-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="4c92e-105">Start Shell til Exchange-administration.</span><span class="sxs-lookup"><span data-stu-id="4c92e-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="4c92e-106">Du kan finde flere oplysninger [i Åbn Shell til Exchange-administration.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="4c92e-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="4c92e-107">Kør denne kommando (ved hjælp af brugerens mailadresse):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="4c92e-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="4c92e-108">Kontrollér, om afsenderens mailadresse er en del af **TrustedSendersAndDomains** eller **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="4c92e-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="4c92e-109">Hvis mailadressen er på en af listerne, skal du muligvis fjerne den.</span><span class="sxs-lookup"><span data-stu-id="4c92e-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="4c92e-110">Du kan få mere at [vide under Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="4c92e-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
