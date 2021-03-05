---
title: Konfiguration af klargøringstjenesten
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481852"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="845d3-102">Konfiguration af klargøringstjenesten</span><span class="sxs-lookup"><span data-stu-id="845d3-102">Configuring the Provision service</span></span>

<span data-ttu-id="845d3-103">For at automatisere klargøring af brugere kan fungere, kræver Azure AD gyldige legitimationsoplysninger, der giver mulighed for at oprette forbindelse til ARBEJDSDAG Web Services API.</span><span class="sxs-lookup"><span data-stu-id="845d3-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="845d3-104">Desuden validerer knappen Testforbindelse på appen Arbejdsdag til AD-bruger klargøring også, om den kan oprette forbindelse til den Azure AD Connect-klargøringsagent, der er knyttet til AD-domænet.</span><span class="sxs-lookup"><span data-stu-id="845d3-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="845d3-105">Hvis Azure-portalen returnerer en fejl, når du gemmer legitimationsoplysningerne, skal du følge de anbefalede trin nedenfor:</span><span class="sxs-lookup"><span data-stu-id="845d3-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="845d3-106">Bekræft, at du har konfigureret arbejdsdagens integrationssystembrugerkonto som nævnt i selvstudiet om konfiguration [af integrationssystembruger i Arbejdsdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="845d3-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="845d3-107">Bekræft, at Azure AD Connect Provisioning Agent Service er oppe at køre på din lokale Windows-server ved hjælp af Services Management Console.</span><span class="sxs-lookup"><span data-stu-id="845d3-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="845d3-108">Du kan også kontrollere status for agenten i Azure-portalen ved at klikke på knappen Vis lokale agenter.</span><span class="sxs-lookup"><span data-stu-id="845d3-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="845d3-109">Sørg for, at du angiver værdien for feltet "Arbejdsdagens brugernavn" ved hjælp username@workday-lejer-navn.</span><span class="sxs-lookup"><span data-stu-id="845d3-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="845d3-110">Hvis navnet på arbejdsdag-lejeren mangler, mislykkes godkendelse af arbejdsdagen.</span><span class="sxs-lookup"><span data-stu-id="845d3-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="845d3-111">Hvis du konfigurerer integrationen med implementeringslejeren for Arbejdsdag, skal du notere de planlagte nedetidstimer for din arbejdsdags lejer.</span><span class="sxs-lookup"><span data-stu-id="845d3-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="845d3-112">Arbejdsdagen har planlagt nedetid for dens implementeringslejere over weekender (som regel fra fredag aften til lørdag morgen), og forbindelsesfejl i denne nedetidsperiode er et kendt problem, der løses automatisk, så snart implementeringslejerne igen er online.</span><span class="sxs-lookup"><span data-stu-id="845d3-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="845d3-113">I sjældne tilfælde får du muligvis også vist denne fejl, hvis adgangskoden til systembrugeren til integration ændres på grund af lejeropdatering, eller hvis kontoen er i låst eller udløbet tilstand.</span><span class="sxs-lookup"><span data-stu-id="845d3-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="845d3-114">Kontrollér status for integrationssystembrugeren med din arbejdsdagsadministrator.</span><span class="sxs-lookup"><span data-stu-id="845d3-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="845d3-115">Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk klargøring af brugere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="845d3-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
