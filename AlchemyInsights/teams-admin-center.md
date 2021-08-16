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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049338"
---
# <a name="teams-admin-center"></a>Teams Administration

Få mere at vide om administration af Teams ved hjælp af [Teams Administration](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke kan få adgang til Teams Administration, skal du kontrollere følgende elementer:

- Kontroller, at du har tilladt de relevante [Office 365-IP-adresser og URL-adresser](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alle perimeterenheder (firewall osv.) eller i firewallreglerne på din lokale computer.
- Bekræft, at det logon, du bruger til at få adgang til Teams Administrationsportal, svarer til dit brugernavn, der er angivet i [Microsoft 365 Administrationsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brugere ikke vises i Teams Administration, skal du kontrollere følgende elementer:

- Har du oprettet brugere eller tildelt licenser inden for de seneste 24 timer? Sørg for at vente mindst 24 timer, før du åbner en supportanmodning.
- Skal du bekræfte, at du har tildelt passende licenser?
- Hvis du har et lokalt Active Directory, skal du bekræfte, at værdien af [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) eller SIP-adressen i feltet ProxyAddresses i dit lokale Active Directory er entydigt, og formatet svarer til **sip:** Brugerens brugernavn [fra Microsoft 365 Administration.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Hvis du har til hensigt at beholde en Skype for Business Server-installation og have brugere lokalt og online: Følg "Konfigurer hybrid med **Teams og Skype for Business Online"** i dit Skype for Business Server Kontrolpanel, og flyt brugere online.
