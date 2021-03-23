---
title: Meddelelse om AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035432"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="099fb-102">Meddelelse om AAD Connect</span><span class="sxs-lookup"><span data-stu-id="099fb-102">Notification AAD Connect</span></span>

- <span data-ttu-id="099fb-103">Sørg for, at du har tilladelse til at udføre handlingen.</span><span class="sxs-lookup"><span data-stu-id="099fb-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="099fb-104">Globale administratorer har som standard adgang.</span><span class="sxs-lookup"><span data-stu-id="099fb-104">Global Admins have access by default.</span></span> <span data-ttu-id="099fb-105">Desuden kan du bruge rollebaseret [adgangskontrol til at](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) uddelegere registreringstilladelse til bidragyderen.</span><span class="sxs-lookup"><span data-stu-id="099fb-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="099fb-106">Sørg for, at de nødvendige slutpunkter er aktiveret og ikke blokeret på grund af firewall.</span><span class="sxs-lookup"><span data-stu-id="099fb-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="099fb-107">Du kan finde flere oplysninger under [krav.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="099fb-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="099fb-108">Registrering kan mislykkes, fordi udgående kommunikation bliver underlagt SSL-inspektion af netværkslaget.</span><span class="sxs-lookup"><span data-stu-id="099fb-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="099fb-109">Sørg for, at du har bekræftet indstillingerne for meddelelser for Azure AD Connect Health, og gennemse din indstilling.</span><span class="sxs-lookup"><span data-stu-id="099fb-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="099fb-110">Se denne vejledning for at forstå, hvordan du konfigurerer meddelelsesindstillingerne for beskeder om Azure AD [Connect-tilstand.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="099fb-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="099fb-111">Hvis du vil have mere at vide om AAD Connect Health-synkroniseringsrapporten, og hvordan du henter den, skal du [se synkroniseringsrapporten på objektniveau.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="099fb-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="099fb-112">Hvis du vil foretage fejlfinding af AAD Connect Health Alerts, skal du følge fejlfindingsvejledningen til beskeder om friskhed [for AAD Connect Health-data](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) og for ofte stillede spørgsmål under [Almindelige installationsspørgsmål om AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="099fb-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
