---
title: 2681 angreb simulator i Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713460"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="70207-102">Angreb simulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="70207-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="70207-103">Mangler du angrebssimulator?</span><span class="sxs-lookup"><span data-stu-id="70207-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="70207-104">Attack Simulator kræver **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="70207-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="70207-105">Attack Simulator er **ikke** inkluderet i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller microsoft 365 Apps til virksomheder-abonnementer.</span><span class="sxs-lookup"><span data-stu-id="70207-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="70207-106">Den konto, du bruger til at starte simulerede angreb, kræver globale administrator- eller sikkerhedsadministratortilladelser og multifaktorgodkendelse.</span><span class="sxs-lookup"><span data-stu-id="70207-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="70207-107">Yderligere oplysninger om kravene til Attack Simulator finder du i [dette emne](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="70207-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="70207-108">Vigtige ting at vide om **Brute Force Password** angreb simuleringer:</span><span class="sxs-lookup"><span data-stu-id="70207-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="70207-109">Hvis målkontoen har aktiveret en MFA, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelsesfaktor vil være ufuldstændig).</span><span class="sxs-lookup"><span data-stu-id="70207-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="70207-110">Adgangskodefilen må ikke være større end 10 MB.</span><span class="sxs-lookup"><span data-stu-id="70207-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="70207-111">Brug én adgangskode pr. linje, og medtag en tom linje (vognretur) efter den sidste adgangskode på listen.</span><span class="sxs-lookup"><span data-stu-id="70207-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="70207-112">Vigtige ting at vide om **Spear Phishing** vedhæfte simuleringer:</span><span class="sxs-lookup"><span data-stu-id="70207-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="70207-113">Efter design kan du ikke angive en brugerdefineret værdi for **URL-adressen til Phishing-loginserveren**.</span><span class="sxs-lookup"><span data-stu-id="70207-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="70207-114">Hvis en modtager bruger [tilføjelsesprogrammet Aktivér rapportmeddelelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (da dette er et simuleret angreb).</span><span class="sxs-lookup"><span data-stu-id="70207-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="70207-115">Rapporter: Når det simulerede angreb er fuldført, kan du klikke på **Angrebsdetaljer** for at se rapporten.</span><span class="sxs-lookup"><span data-stu-id="70207-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="70207-116">Yderligere oplysninger og nye funktioner i Attack Simulator finder du i [Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="70207-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
