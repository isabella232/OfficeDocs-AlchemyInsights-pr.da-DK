---
title: 2681 angreb simulator i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305326"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="062df-102">Angrebs simulator i Office 365</span><span class="sxs-lookup"><span data-stu-id="062df-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="062df-103">Er du mangler angreb Simulator?</span><span class="sxs-lookup"><span data-stu-id="062df-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="062df-104">Angrebs simulator kræver **office 365 Advanced Threat Protection plan 2 (ATP plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="062df-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="062df-105">Angrebs Simulator er **ikke** inkluderet i Office 365 Advanced Threat Protection plan 1 (ATP plan 1), Office 365 Enterprise E3 eller et Office 365 Business-abonnement.</span><span class="sxs-lookup"><span data-stu-id="062df-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="062df-106">Den konto, du bruger til at starte simulerede angreb, kræver global administrator-eller sikkerhedsadministrator tilladelser og multifaktorgodkendelse (MFA).</span><span class="sxs-lookup"><span data-stu-id="062df-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="062df-107">Du finder flere oplysninger om angrebs simulator krav i [dette emne](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="062df-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="062df-108">Vigtige ting at vide om **Brute Force password** angreb simuleringer:</span><span class="sxs-lookup"><span data-stu-id="062df-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="062df-109">Hvis der er aktiveret MFA på målkontoen, og adgangskoden blev gættet korrekt, vil kontoen ikke blive vist som kompromitteret (den anden godkendelses faktor vil være ufuldstændig).</span><span class="sxs-lookup"><span data-stu-id="062df-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="062df-110">Adgangskodefilen må ikke være større end 10 MB.</span><span class="sxs-lookup"><span data-stu-id="062df-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="062df-111">Brug én adgangskode pr. linje, og Medtag en tom linje (vognretur) efter den sidste adgangskode på listen.</span><span class="sxs-lookup"><span data-stu-id="062df-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="062df-112">Vigtige ting at vide om **Spear phishing** vedhæfte simuleringer:</span><span class="sxs-lookup"><span data-stu-id="062df-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="062df-113">Ved design kan du ikke angive en brugerdefineret værdi for **phishing-logonserverens webadresse**.</span><span class="sxs-lookup"><span data-stu-id="062df-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="062df-114">Hvis en modtager bruger funktionen [Aktivér rapport meddelelsen](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke påmindelser om meddelelsen (fordi dette er et simuleret angreb).</span><span class="sxs-lookup"><span data-stu-id="062df-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="062df-115">Rapporter: når det simulerede angreb er fuldført, kan du klikke på **angrebs detaljer** for at se rapporten.</span><span class="sxs-lookup"><span data-stu-id="062df-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="062df-116">For detaljerede instruktioner og nye funktioner i Attack simulator, se [Attack simulator i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="062df-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
