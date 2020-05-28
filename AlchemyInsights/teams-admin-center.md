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
# <a name="teams-admin-center"></a>Teams Administration

Få mere at vide om administration af Teams ved hjælp af [Teams Administration](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke kan få adgang til Teams Administration, skal du kontrollere følgende elementer:

- Kontroller, at du har tilladt de relevante [Office 365-IP-adresser og URL-adresser](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alle perimeterenheder (firewall osv.) eller i firewallreglerne på din lokale computer.
- Bekræft, at det logon, du bruger til at få adgang til Teams Administrationsportal, svarer til dit brugernavn, der er angivet i [Microsoft 365 Administrationsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brugere ikke vises i Teams Administration, skal du kontrollere følgende elementer:

- Har du oprettet brugere eller tildelt licenser inden for de seneste 24 timer? Sørg for at vente mindst 24 timer, før du åbner en supportanmodning.
- Skal du bekræfte, at du har tildelt passende licenser?
- Hvis du har et lokalt Active Directory, skal du kontrollere, at [værdien af msRTCSIP-PrimaryUserAddress eller SIP-adressen i feltet ProxyAddresses i dit lokale Active Directory er entydigt, og formatet svarer til](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Brugerens brugernavn** fra Microsoft [365 Administration](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Hvis du vil beholde en Skype for Business Server-installation og få brugerne til at være hjemme og online: Følg **"Konfigurer hybrid med Teams og Skype for Business Online"** i kontrolpanelet på Skype for Business Server, og flyt brugere online.
