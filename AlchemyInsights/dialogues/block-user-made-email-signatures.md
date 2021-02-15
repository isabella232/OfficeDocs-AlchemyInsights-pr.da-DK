---
title: Blokere brugerbaserede mailsignaturer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243318"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="d305f-102">Blokere brugerbaserede mailsignaturer</span><span class="sxs-lookup"><span data-stu-id="d305f-102">Block user-made email signatures</span></span>

<span data-ttu-id="d305f-103">Følgende løsning gælder kun for mailsignaturer, der er oprettet i Outlook på internettet.</span><span class="sxs-lookup"><span data-stu-id="d305f-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="d305f-104">Du kan kun blokere signaturer i Outlook-appen, hvis du har en lokal Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="d305f-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="d305f-105">Vælg Administration Exchange **i**  >  **Administration.**</span><span class="sxs-lookup"><span data-stu-id="d305f-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="d305f-106">Klik **på tilladelser i** Outlook Web  >  **App-politikker.**</span><span class="sxs-lookup"><span data-stu-id="d305f-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="d305f-107">Vælg politikken, og klik derefter på blyantsikonet for at redigere den.</span><span class="sxs-lookup"><span data-stu-id="d305f-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="d305f-108">Klik **på funktioner** Flere  >  **indstillinger.**</span><span class="sxs-lookup"><span data-stu-id="d305f-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="d305f-109">Fjern **markeringen i afkrydsningsfeltet** **Mailsignatur under** Brugeroplevelse, og klik derefter på **Gem.**</span><span class="sxs-lookup"><span data-stu-id="d305f-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="d305f-110">**Vigtigt!** Hvis der blev tilføjet en signatur, før dette afkrydsningsfelt blev fjernet, vil brugeren stadig kunne bruge den.</span><span class="sxs-lookup"><span data-stu-id="d305f-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="d305f-111">Bed dem om at fjerne den.</span><span class="sxs-lookup"><span data-stu-id="d305f-111">Ask them to remove it.</span></span>
