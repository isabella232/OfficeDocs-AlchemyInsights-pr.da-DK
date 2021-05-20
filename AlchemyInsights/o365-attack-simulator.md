---
title: 2681 Attack– – – Microsoft 365
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545720"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="9fd31-102">Angrebs in-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9fd31-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="9fd31-103">Går du glip af Angrebs problem?</span><span class="sxs-lookup"><span data-stu-id="9fd31-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="9fd31-104">Attack Defender kræver **Microsoft Defender til Office 365 Plan 2** eller Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="9fd31-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="9fd31-105">Attack Defender er **ikke** inkluderet i Microsoft Defender Office 365 Plan 1, Office 365 Enterprise E3 eller nogen Microsoft 365 Apps for business abonnementer.</span><span class="sxs-lookup"><span data-stu-id="9fd31-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="9fd31-106">Den konto, du bruger til at starte simulerede angreb, kræver globale administrator- eller sikkerhedsadministratortilladelser og multifaktorgodkendelse.</span><span class="sxs-lookup"><span data-stu-id="9fd31-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="9fd31-107">Du kan finde flere oplysninger om krav til angrebsspil i [dette emne](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="9fd31-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="9fd31-108">Vigtige ting at vide om **Brute Force-angrebssimulering** af adgangskoder:</span><span class="sxs-lookup"><span data-stu-id="9fd31-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="9fd31-109">Hvis målkontoen har MFA aktiveret, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelsesfaktor vil være ufuldstændig).</span><span class="sxs-lookup"><span data-stu-id="9fd31-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="9fd31-110">Adgangskodefilen må ikke være større end 10 MB.</span><span class="sxs-lookup"><span data-stu-id="9fd31-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="9fd31-111">Brug én adgangskode pr. linje, og medtag en tom linje (vognretur) efter den sidste adgangskode på listen.</span><span class="sxs-lookup"><span data-stu-id="9fd31-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="9fd31-112">Vigtige ting, du skal vide om **phishing-phishing, som** vedhæfter simulering:</span><span class="sxs-lookup"><span data-stu-id="9fd31-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="9fd31-113">Du kan ikke angive en brugerdefineret værdi for URL-adresse til **phishing-loginserver.**</span><span class="sxs-lookup"><span data-stu-id="9fd31-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="9fd31-114">Hvis en modtager [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) bruger tilføjelsesprogrammet Aktivér rapportmeddelelse for at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (da dette er et simuleret angreb).</span><span class="sxs-lookup"><span data-stu-id="9fd31-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="9fd31-115">Rapporter: Når de simulerede angreb er udført, kan du klikke **på Oplysninger om angreb** for at få vist rapporten.</span><span class="sxs-lookup"><span data-stu-id="9fd31-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="9fd31-116">Hvis du vil have detaljeret vejledning og nye funktioner i Angrebsangreb, skal [du se Angrebs muligheder Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="9fd31-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
