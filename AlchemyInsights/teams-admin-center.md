---
title: Teams Administration
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826373"
---
# <a name="teams-admin-center"></a>Teams Administration

Få mere at vide om administration af Teams ved hjælp af [Teams Administration](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke kan få adgang til Teams Administration, skal du kontrollere følgende elementer:

- Kontroller, at du har tilladt de relevante [Office 365-IP-adresser og URL-adresser](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alle perimeterenheder (firewall osv.) eller i firewallreglerne på din lokale computer.
- Bekræft, at det logon, du bruger til at få adgang til Teams Administrationsportal, svarer til dit brugernavn, der er angivet i [Microsoft 365 Administrationsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brugere ikke vises i Teams Administration, skal du kontrollere følgende elementer:

- Har du oprettet brugere eller tildelt licenser inden for de seneste 24 timer? Sørg for at vente mindst 24 timer, før du åbner en supportanmodning.
- Skal du bekræfte, at du har tildelt passende licenser?
- Hvis du har et lokalt Active Directory, skal du bekræfte, at værdien af [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) eller SIP-adressen i feltet ProxyAddresses i dit lokale Active Directory er entydigt, og formatet svarer til **sip:** Brugerens brugernavn fra [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)Administration.
- Hvis du vil beholde en Skype for Business Server-installation og have brugere lokalt og online: Følg "Konfigurer hybrid med Teams og **Skype for Business Online"** i kontrolpanelet i Skype for Business Server, og flyt brugere online.
