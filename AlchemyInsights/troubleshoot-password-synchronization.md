---
title: Fejlfinding i forbindelse med synkronisering af adgangskoder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732504"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="8002e-102">Fejlfinding i forbindelse med synkronisering af adgangskoder</span><span class="sxs-lookup"><span data-stu-id="8002e-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="8002e-103">Sådan foretager du fejlfinding af problemer, hvor der ikke synkroniseres adgangskoder med Azure AD Connect version 1.1.614.0 eller nyere:</span><span class="sxs-lookup"><span data-stu-id="8002e-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="8002e-104">Åbn en ny Windows PowerShell-session på Azure AD Connect-serveren med indstillingen **Kør som administrator.**</span><span class="sxs-lookup"><span data-stu-id="8002e-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="8002e-105">Kør **Set-ExecutionPolicy RemoteSigned** eller **Set-ExecutionPolicy Ubegrænset**.</span><span class="sxs-lookup"><span data-stu-id="8002e-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="8002e-106">Start guiden Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8002e-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="8002e-107">Gå til siden **Flere opgaver,** vælg **Fejlfinding**, og klik på **Næste**.</span><span class="sxs-lookup"><span data-stu-id="8002e-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="8002e-108">Klik på Start på siden Fejlfinding **for at starte fejlfindingsmenuen** i PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8002e-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="8002e-109">Vælg Fejlfinding af **synkronisering af adgangskoder i**hovedmenuen .</span><span class="sxs-lookup"><span data-stu-id="8002e-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="8002e-110">I undermenuen skal du vælge **Password Synkronisering virker slet ikke**.</span><span class="sxs-lookup"><span data-stu-id="8002e-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="8002e-111">**Forstå resultaterne af fejlfindingsopgaven**</span><span class="sxs-lookup"><span data-stu-id="8002e-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="8002e-112">Fejlfindingsopgaven udfører følgende kontroller:</span><span class="sxs-lookup"><span data-stu-id="8002e-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="8002e-113">Validerer, at funktionen til synkronisering af adgangskoder er aktiveret for din Azure AD-lejer.</span><span class="sxs-lookup"><span data-stu-id="8002e-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="8002e-114">Kontrollerer, at Azure AD Connect-serveren ikke er i midlertidig tilstand.</span><span class="sxs-lookup"><span data-stu-id="8002e-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="8002e-115">For hver eksisterende Active Directory-forbindelse i det lokale miljø (hvilket svarer til et eksisterende Active Directory-område):</span><span class="sxs-lookup"><span data-stu-id="8002e-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="8002e-116">Kontrollerer, at funktionen til synkronisering af adgangskoder er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="8002e-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="8002e-117">Søger efter hjertestartere til synkronisering af adgangskoder i Windows Application Event-logfilerne.</span><span class="sxs-lookup"><span data-stu-id="8002e-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="8002e-118">For hvert Active Directory-domæne under den lokale Active Directory-forbindelse:</span><span class="sxs-lookup"><span data-stu-id="8002e-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="8002e-119">Validerer, at domænet kan nås fra Azure AD Connect-serveren.</span><span class="sxs-lookup"><span data-stu-id="8002e-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="8002e-120">Kontrollerer, at de AD DS-konti (Active Directory Domain Services), der bruges af det lokale Active Directory-stik, har det korrekte brugernavn, den korrekte adgangskode og de tilladelser, der kræves til synkronisering af adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="8002e-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="8002e-121">Du kan få mere hjælp til fejlfinding af synkronisering af adgangskoder [under Fejlfinding af synkronisering af adgangskoder med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="8002e-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  