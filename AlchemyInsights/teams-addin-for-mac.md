---
title: Teams-tilføjelsesprogrammet til Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582064"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="e51af-102">Teams-tilføjelsesprogrammet til Mac</span><span class="sxs-lookup"><span data-stu-id="e51af-102">Teams add-in for Mac</span></span>

<span data-ttu-id="e51af-103">Hvis du vil foretage fejlfinding Teams til tilføjelsesprogrammet til Mac-operativsystemets brugere, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="e51af-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="e51af-104">**Trin 1:** Hvis du har en Exchange lokal (2016 CU3 eller nyere påkrævet), skal du bruge værktøjet Test-HMA.ps1 til at bekræfte, at hybrid moderne godkendelse er konfigureret korrekt.</span><span class="sxs-lookup"><span data-stu-id="e51af-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="e51af-105">Du kan få mere at vide [under Validering af konfiguration af hybrid moderne godkendelse Outlook til iOS og Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="e51af-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="e51af-106">**Bemærk!** Brug UPN-adresseformatet (f.eks. [username@contoso.com](mailto:username@contoso.com)), ikke domæne\brugernavn.</span><span class="sxs-lookup"><span data-stu-id="e51af-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="e51af-107">Gør dette selv for brugere med Exchange Online postkasser.</span><span class="sxs-lookup"><span data-stu-id="e51af-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="e51af-108">**Trin 2:** Få brugeren til at gå **til**  >  **Værktøjskonti**... i Outlook til Mac, og find og vælg kontoen.</span><span class="sxs-lookup"><span data-stu-id="e51af-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="e51af-109">Bekræft, at det angivne brugernavn er i UPN-format (f.eks. [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="e51af-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="e51af-110">**Trin 3:** Bekræft, at brugeren er en Microsoft Teams bruger.</span><span class="sxs-lookup"><span data-stu-id="e51af-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="e51af-111">Brugeren skal bruge abonnementet Office 365 til Mac, produktversion 16.24 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="e51af-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>