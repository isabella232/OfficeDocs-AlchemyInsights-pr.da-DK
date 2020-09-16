---
title: Teams Administration
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670358"
---
# <a name="teams-admin-center"></a><span data-ttu-id="ddfe9-102">Teams Administration</span><span class="sxs-lookup"><span data-stu-id="ddfe9-102">Teams Admin Center</span></span>

<span data-ttu-id="ddfe9-103">Få mere at vide om administration af Teams ved hjælp af [Teams Administration](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="ddfe9-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="ddfe9-104">Hvis du ikke kan få adgang til Teams Administration, skal du kontrollere følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="ddfe9-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="ddfe9-105">Kontroller, at du har tilladt de relevante [Office 365-IP-adresser og URL-adresser](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alle perimeterenheder (firewall osv.) eller i firewallreglerne på din lokale computer.</span><span class="sxs-lookup"><span data-stu-id="ddfe9-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="ddfe9-106">Bekræft, at det logon, du bruger til at få adgang til Teams Administrationsportal, svarer til dit brugernavn, der er angivet i [Microsoft 365 Administrationsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="ddfe9-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="ddfe9-107">Hvis brugere ikke vises i Teams Administration, skal du kontrollere følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="ddfe9-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="ddfe9-108">Har du oprettet brugere eller tildelt licenser inden for de seneste 24 timer?</span><span class="sxs-lookup"><span data-stu-id="ddfe9-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="ddfe9-109">Sørg for at vente mindst 24 timer, før du åbner en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="ddfe9-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="ddfe9-110">Skal du bekræfte, at du har tildelt passende licenser?</span><span class="sxs-lookup"><span data-stu-id="ddfe9-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="ddfe9-111">Hvis du har et lokalt Active Directory, skal du kontrollere, at [værdien af msRTCSIP-PrimaryUserAddress eller SIP-adressen i proxyAddresses-feltet i dit lokale Active Directory er entydigt, og formatet stemmer](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) overens med SIP: bruger**navn** fra [Microsoft 365 administration](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="ddfe9-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="ddfe9-112">Hvis du har tænkt dig at beholde en Skype for Business Server-installation og har brugere, der har hjem, online, skal du følge indstillingen **"konfigurere hybrid med teams og Skype for Business online"** i din Skype for Business Server-kontrol panel og flytte brugere online.</span><span class="sxs-lookup"><span data-stu-id="ddfe9-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
