---
title: Eksempel på politik for Sikker vedhæftet fil i Microsoft Defender til Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693100"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="b998c-102">Eksempel på politik for Sikker vedhæftet fil i Microsoft Defender til Office 365</span><span class="sxs-lookup"><span data-stu-id="b998c-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="b998c-103">Disse indstillinger aktiverer en politik kaldet *Ingen forsinkelser,* der leverer meddelelser med det samme og derefter vedhæftede filer igen, når de er scannet:</span><span class="sxs-lookup"><span data-stu-id="b998c-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="b998c-104">**Navn:** Ingen forsinkelser</span><span class="sxs-lookup"><span data-stu-id="b998c-104">**Name**: No delays</span></span>
- <span data-ttu-id="b998c-105">**Beskrivelse:** Leverer meddelelser straks og vedhæftede filer igen efter scanning.</span><span class="sxs-lookup"><span data-stu-id="b998c-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="b998c-106">**Svar:** Vælg **indstillingen Dynamisk** levering.</span><span class="sxs-lookup"><span data-stu-id="b998c-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="b998c-107">Du kan finde flere oplysninger i [Dynamisk levering i politikker for sikre vedhæftede filer.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="b998c-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="b998c-108">**Omdiriger** sektionen vedhæftede filer: Vælg indstillingen til at aktivere **omdirigering,** og angiv derefter mailadressen på den globale Microsoft 365-administrator, sikkerhedsadministrator eller sikkerhedsanalytiker, der vil undersøge skadelige vedhæftede filer.</span><span class="sxs-lookup"><span data-stu-id="b998c-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="b998c-109">**Anvendt på** sektion: Vælg **modtagerdomænet,** og vælg derefter dit domæne.</span><span class="sxs-lookup"><span data-stu-id="b998c-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="b998c-110">Vælg **Tilføj,** og vælg derefter **OK.**</span><span class="sxs-lookup"><span data-stu-id="b998c-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="b998c-111">Vælg Gem, når du er **færdig.**</span><span class="sxs-lookup"><span data-stu-id="b998c-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="b998c-112">Du kan få mere at vide [under Sikre vedhæftede filer i Microsoft Defender til Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="b998c-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
