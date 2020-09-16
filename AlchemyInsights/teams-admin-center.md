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
# <a name="teams-admin-center"></a>Teams Administration

Få mere at vide om administration af Teams ved hjælp af [Teams Administration](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke kan få adgang til Teams Administration, skal du kontrollere følgende elementer:

- Kontroller, at du har tilladt de relevante [Office 365-IP-adresser og URL-adresser](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alle perimeterenheder (firewall osv.) eller i firewallreglerne på din lokale computer.
- Bekræft, at det logon, du bruger til at få adgang til Teams Administrationsportal, svarer til dit brugernavn, der er angivet i [Microsoft 365 Administrationsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brugere ikke vises i Teams Administration, skal du kontrollere følgende elementer:

- Har du oprettet brugere eller tildelt licenser inden for de seneste 24 timer? Sørg for at vente mindst 24 timer, før du åbner en supportanmodning.
- Skal du bekræfte, at du har tildelt passende licenser?
- Hvis du har et lokalt Active Directory, skal du kontrollere, at [værdien af msRTCSIP-PrimaryUserAddress eller SIP-adressen i proxyAddresses-feltet i dit lokale Active Directory er entydigt, og formatet stemmer](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) overens med SIP: bruger**navn** fra [Microsoft 365 administration](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Hvis du har tænkt dig at beholde en Skype for Business Server-installation og har brugere, der har hjem, online, skal du følge indstillingen **"konfigurere hybrid med teams og Skype for Business online"** i din Skype for Business Server-kontrol panel og flytte brugere online.
