---
title: Beskyttelse mod Backscatter-angreb
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035409"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="57675-102">Beskyttelse mod Backscatter-angreb</span><span class="sxs-lookup"><span data-stu-id="57675-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="57675-103">Backscatter er rapporter om manglende levering (også kaldet rapporter om manglende levering eller meddelelser om ikke-leveret mail), som du modtager for meddelelser, du ikke har sendt.</span><span class="sxs-lookup"><span data-stu-id="57675-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="57675-104">Afsendere af uønsket mail (spoof) **Fra:-adressen** på deres meddelelser, og de bruger ofte reelle mailadresser til at give deres meddelelser troværdighed.</span><span class="sxs-lookup"><span data-stu-id="57675-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="57675-105">Så når spammere uundgåeligt sender meddelelser til ikke-eksisterende modtagere, bliver destinationsmailserveren i bund og grund narret til at returnere den meddelelse, der ikke kan leveres, i en NDR til den smedede afsender i **Fra:-adressen.**</span><span class="sxs-lookup"><span data-stu-id="57675-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="57675-106">Du kan finde flere oplysninger [i Backscatter i EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="57675-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="57675-107">**Aktivering af Backscatter-beskyttelse**</span><span class="sxs-lookup"><span data-stu-id="57675-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="57675-108">Følg stien nedenfor for at aktivere Backscatter-beskyttelse.</span><span class="sxs-lookup"><span data-stu-id="57675-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="57675-109">**protection.office.com > trusselsadministration > politik > antispam > Vælg politik for spamfilter og rediger politik > egenskaber > Spam > Markér som spam > NDR-backscatter > Indstil den til "Til"**</span><span class="sxs-lookup"><span data-stu-id="57675-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="57675-110">Hvis du mener, at en konto er blevet kompromitteret, skal du se følgende:</span><span class="sxs-lookup"><span data-stu-id="57675-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="57675-111">Besvare en kompromitteret mailkonto</span><span class="sxs-lookup"><span data-stu-id="57675-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="57675-112">Fjerne blokerede brugere fra portalen Begrænsede brugere i Office 365</span><span class="sxs-lookup"><span data-stu-id="57675-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



