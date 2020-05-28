---
title: Teams Administration
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354082"
---
# <a name="teams-admin-center"></a><span data-ttu-id="cd1e2-102">Teams Administration</span><span class="sxs-lookup"><span data-stu-id="cd1e2-102">Teams Admin Center</span></span>

<span data-ttu-id="cd1e2-103">Få mere at vide om administration af Teams ved hjælp af [Teams Administration](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="cd1e2-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="cd1e2-104">Hvis du ikke kan få adgang til Teams Administration, skal du kontrollere følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="cd1e2-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="cd1e2-105">Kontroller, at du har tilladt de relevante [Office 365-IP-adresser og URL-adresser](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alle perimeterenheder (firewall osv.) eller i firewallreglerne på din lokale computer.</span><span class="sxs-lookup"><span data-stu-id="cd1e2-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="cd1e2-106">Bekræft, at det logon, du bruger til at få adgang til Teams Administrationsportal, svarer til dit brugernavn, der er angivet i [Microsoft 365 Administrationsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="cd1e2-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="cd1e2-107">Hvis brugere ikke vises i Teams Administration, skal du kontrollere følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="cd1e2-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="cd1e2-108">Har du oprettet brugere eller tildelt licenser inden for de seneste 24 timer?</span><span class="sxs-lookup"><span data-stu-id="cd1e2-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="cd1e2-109">Sørg for at vente mindst 24 timer, før du åbner en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="cd1e2-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="cd1e2-110">Skal du bekræfte, at du har tildelt passende licenser?</span><span class="sxs-lookup"><span data-stu-id="cd1e2-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="cd1e2-111">Hvis du har et lokalt Active Directory, skal du kontrollere, at [værdien af msRTCSIP-PrimaryUserAddress eller SIP-adressen i feltet ProxyAddresses i dit lokale Active Directory er entydigt, og formatet svarer til](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Brugerens brugernavn** fra Microsoft [365 Administration](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="cd1e2-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="cd1e2-112">Hvis du vil beholde en Skype for Business Server-installation og få brugerne til at være hjemme og online: Følg **"Konfigurer hybrid med Teams og Skype for Business Online"** i kontrolpanelet på Skype for Business Server, og flyt brugere online.</span><span class="sxs-lookup"><span data-stu-id="cd1e2-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
