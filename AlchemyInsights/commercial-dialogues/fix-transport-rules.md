---
title: Ret transportregler
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744845"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="3e78c-102">Ret transportregler</span><span class="sxs-lookup"><span data-stu-id="3e78c-102">Fix transport rules</span></span>

<span data-ttu-id="3e78c-103">En brugerdefineret regel for mailflow påvirkede denne meddelelse.</span><span class="sxs-lookup"><span data-stu-id="3e78c-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="3e78c-104">Hvis du vil gennemse den nøjagtige regel, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="3e78c-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="3e78c-105">Under Yderligere oplysninger skal du **notere** **GUID'et** eller **politiknavnet i indsendelsesresultaterne.**</span><span class="sxs-lookup"><span data-stu-id="3e78c-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="3e78c-106">Start Shell til Exchange-administration.</span><span class="sxs-lookup"><span data-stu-id="3e78c-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="3e78c-107">Du kan finde flere oplysninger [i Åbn Shell til Exchange-administration.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="3e78c-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="3e78c-108">Kør denne kommando (ved hjælp af GUID fra din indsendelse):  **Get-TransportRule -identity "GUID" | fl \* Beskrivelse**\*</span><span class="sxs-lookup"><span data-stu-id="3e78c-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="3e78c-109">Gennemgå beskrivelsen for at se de konfigurerede betingelser, der har påvirket meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="3e78c-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="3e78c-110">Du kan få mere at vide [under Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="3e78c-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
