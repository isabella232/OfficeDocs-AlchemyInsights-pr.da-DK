---
title: 2681-angrebs simulator i Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759213"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="b7f15-102">Angrebs simulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b7f15-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="b7f15-103">Mangler du angrebs Simulator?</span><span class="sxs-lookup"><span data-stu-id="b7f15-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b7f15-104">Angrebs simulator kræver **Office 365 Advanced Threat Protection plan 2 (DTT-plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="b7f15-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b7f15-105">Angrebs Simulator er **ikke** inkluderet i Office 365 Advanced Threat Protection plan 1 (DTT plan 1), Office 365 Enterprise E3 eller eventuelle Microsoft 365-apps til virksomheds abonnementer.</span><span class="sxs-lookup"><span data-stu-id="b7f15-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="b7f15-106">Den konto, du bruger til at køre simulerede angreb, kræver globale administrator-eller sikkerhedsadministrator tilladelser og multifaktorgodkendelse (MFA).</span><span class="sxs-lookup"><span data-stu-id="b7f15-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b7f15-107">Hvis du vil have mere at vide om krav til angrebs simulator, skal du se [dette emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b7f15-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="b7f15-108">Vigtige ting, du skal vide om **Brute Gennemtving** simulerede adgangskode angreb:</span><span class="sxs-lookup"><span data-stu-id="b7f15-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b7f15-109">Hvis destinationskontoen er MFA aktiveret, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelses faktor er ufuldstændig).</span><span class="sxs-lookup"><span data-stu-id="b7f15-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b7f15-110">Adgangskodefilen må ikke være større end 10 MB.</span><span class="sxs-lookup"><span data-stu-id="b7f15-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b7f15-111">Brug én adgangskode pr. linje, og Medtag en tom linje (vognretur) efter den sidste adgangskode på listen.</span><span class="sxs-lookup"><span data-stu-id="b7f15-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b7f15-112">Vigtige ting, du skal vide om **Spear phishing** -tilkoblings simuleringer:</span><span class="sxs-lookup"><span data-stu-id="b7f15-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b7f15-113">Du kan ikke angive en brugerdefineret værdi til **URL-adressen til phishing-logonserveren**.</span><span class="sxs-lookup"><span data-stu-id="b7f15-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b7f15-114">Hvis en modtager bruger funktionen [Aktivér tilføjelse af rapport meddelelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (fordi dette er et simuleret angreb).</span><span class="sxs-lookup"><span data-stu-id="b7f15-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b7f15-115">Rapporter: når det simulerede angreb er fuldført, kan du klikke på **oplysninger om angreb** for at få vist rapporten.</span><span class="sxs-lookup"><span data-stu-id="b7f15-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b7f15-116">Du kan få mere at vide om de nye funktioner i angrebs simulatoren under [angrebs simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b7f15-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
