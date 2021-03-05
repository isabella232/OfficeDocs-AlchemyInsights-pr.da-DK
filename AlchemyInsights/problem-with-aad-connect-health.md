---
title: Problem med AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481464"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="2a3a0-102">Problem med AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="2a3a0-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="2a3a0-103">Sørg for, at du har tilladelse til at udføre handlingen.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="2a3a0-104">Globale administratorer har som standard adgang.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-104">Global Admins have access by default.</span></span> <span data-ttu-id="2a3a0-105">Desuden kan du bruge rollebaseret [adgangskontrol til at](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) uddelegere registreringstilladelse til bidragyderen.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="2a3a0-106">Sørg for, at de nødvendige slutpunkter er aktiveret og ikke blokeret på grund af firewallen.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="2a3a0-107">Du kan finde flere oplysninger under [krav.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="2a3a0-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="2a3a0-108">Registrering kan mislykkes, fordi udgående kommunikation bliver underlagt SSL-inspektion af netværkslaget.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="2a3a0-109">Sørg for, at du har bekræftet indstillingerne for meddelelser for Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="2a3a0-110">Gennemse din indstilling.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-110">Please review your setting.</span></span> <span data-ttu-id="2a3a0-111">Denne [vejledning kan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) hjælpe dig med at forstå, hvordan du konfigurerer meddelelsesindstillingerne for Azure AD Connect-tilstandsmeddelelser.</span><span class="sxs-lookup"><span data-stu-id="2a3a0-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="2a3a0-112">Du kan få mere at vide om AAD Connect Health-synkroniseringsrapporten, og hvordan du henter den, i [rapporten Objektniveausynkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="2a3a0-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="2a3a0-113">Hvis du vil foretage fejlfinding af AAD Connect Health-beskeder, skal du følge fejlfindingsvejledningen til beskeder om, hvor vigtige [AAD Connect Health-data](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) er, og om ofte stillede spørgsmål, skal du se almindelige [installationsspørgsmål om AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="2a3a0-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
