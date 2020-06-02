---
title: 2681 Angreb Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506732"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="1e6ca-102">Angreb Simulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1e6ca-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="1e6ca-103">Er du mangler Angreb Simulator?</span><span class="sxs-lookup"><span data-stu-id="1e6ca-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="1e6ca-104">Angrebssimulator kræver **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="1e6ca-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="1e6ca-105">Attack Simulator er **ikke** inkluderet i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller microsoft 365 Apps til virksomheder-abonnementer.</span><span class="sxs-lookup"><span data-stu-id="1e6ca-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="1e6ca-106">Den konto, du bruger til at starte simulerede angreb, kræver globale administrator- eller sikkerhedsadministratortilladelser og MFA (multifaktorgodkendelse).</span><span class="sxs-lookup"><span data-stu-id="1e6ca-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="1e6ca-107">Yderligere oplysninger om krav til angrebssimulator finder du i [dette emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1e6ca-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="1e6ca-108">Vigtige ting at vide om **Brute Force Password** angreb simuleringer:</span><span class="sxs-lookup"><span data-stu-id="1e6ca-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="1e6ca-109">Hvis målkontoen har aktiveret MFA, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelsesfaktor vil være ufuldstændig).</span><span class="sxs-lookup"><span data-stu-id="1e6ca-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="1e6ca-110">Adgangskodefilen må ikke være større end 10 MB.</span><span class="sxs-lookup"><span data-stu-id="1e6ca-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="1e6ca-111">Brug én adgangskode pr. linje, og medtag en tom linje (vognretur) efter den sidste adgangskode på listen.</span><span class="sxs-lookup"><span data-stu-id="1e6ca-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="1e6ca-112">Vigtige ting at vide om **Spear Phishing** vedhæfte simuleringer:</span><span class="sxs-lookup"><span data-stu-id="1e6ca-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="1e6ca-113">Efter design kan du ikke angive en brugerdefineret værdi for **URL-adressen til phishing-loginserveren**.</span><span class="sxs-lookup"><span data-stu-id="1e6ca-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="1e6ca-114">Hvis en modtager bruger [tilføjelsesprogrammet Aktivér rapportmeddelelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (fordi dette er et simuleret angreb).</span><span class="sxs-lookup"><span data-stu-id="1e6ca-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="1e6ca-115">Rapporter: Når det simulerede angreb er fuldført, kan du klikke på **Angrebsoplysninger** for at se rapporten.</span><span class="sxs-lookup"><span data-stu-id="1e6ca-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="1e6ca-116">Yderligere oplysninger og nye funktioner i Attack Simulator finder du i [Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1e6ca-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
