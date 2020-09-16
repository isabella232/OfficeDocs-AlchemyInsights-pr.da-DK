---
title: Teams-tilføjelsesprogram til Mac
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670322"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="bb0bf-102">Teams-tilføjelsesprogram til Mac</span><span class="sxs-lookup"><span data-stu-id="bb0bf-102">Teams add-in for Mac</span></span>

<span data-ttu-id="bb0bf-103">Hvis du vil foretage fejlfinding af et manglende teams-tilføjelsesprogram til Mac-operativsystem, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="bb0bf-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="bb0bf-104">**Trin 1:** Hvis du har hybrid Exchange i det lokale miljø (2016 CU3 eller senere påkrævet), skal du bruge Test-HMA.ps1s værktøjet til at bekræfte, at hybrid moderne godkendelse er konfigureret korrekt.</span><span class="sxs-lookup"><span data-stu-id="bb0bf-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="bb0bf-105">Hvis du vil have mere at vide, skal du se [validere hybrid installation af moderne godkendelse til Outlook til iOS og Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="bb0bf-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="bb0bf-106">**Bemærk!** Brug UPN-adresseformatet (f. eks. [username@contoso.com](mailto:username@contoso.com)), ikke DOMAIN\USERNAME.</span><span class="sxs-lookup"><span data-stu-id="bb0bf-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="bb0bf-107">Gør dette selv for brugere med Exchange Online-postkasser.</span><span class="sxs-lookup"><span data-stu-id="bb0bf-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="bb0bf-108">**Trin 2:** Få brugeren til at gå til **værktøjer**-  >  **konti**... i Outlook til Mac og finde og vælge kontoen.</span><span class="sxs-lookup"><span data-stu-id="bb0bf-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="bb0bf-109">Bekræft, at det Brugernavn, der er angivet, er i UPN-formatet (f. eks. [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="bb0bf-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="bb0bf-110">**Trin 3:** Bekræft, at brugeren er licenseret af Microsoft teams-brugere.</span><span class="sxs-lookup"><span data-stu-id="bb0bf-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="bb0bf-111">Brugeren skal bruge Office 365 til Mac-abonnement, produktversion 16,24 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="bb0bf-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>