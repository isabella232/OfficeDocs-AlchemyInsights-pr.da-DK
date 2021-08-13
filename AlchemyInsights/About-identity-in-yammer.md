---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918931"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Det anbefales, at alle netværk gør følgende for at undgå identitetsrelaterede problemer:

1. Gennemtving Office 365 efter klargøring af Microsoft 365-konti til brugere i Azure AD for at sikre, at alle brugere logger på ved hjælp af deres primære Microsoft 365-konto. Du kan få mere at vide [under Gennemtving Office 365 identitet for Yammer brugere.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Konsolider flere Yammer netværk. Ældre Yammer konfigurationer tillader flere Yammer netværk at blive forbundet til én lejer. Du kan få mere at vide [under Netværksoverførsel – Konsolider flere Yammer netværk.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Du kan også gennemtvinge licensering for Yammer at blokere brugere fra Yammer hvis de ikke har en licens. Du kan få mere at [vide under Yammer brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Til sidst skal du overvåge brugerlisten for ældre Yammer ældre netværk og suspendere ældre brugere. Det anbefales, at du suspenderer (deaktiverer) brugere i stedet for at slette dem, fordi sletningen ikke kan fortrydes. Få mere at vide under Overvågning [af Yammer brugere i netværk, der er forbundet Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og Fjern [brugere.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Når du konfigurerer Yammer ved hjælp af disse trin, er du også klar til at konfigurere dit Yammer for indbygget tilstand for Microsoft 365. Du kan få mere at [vide under Konfigurere Yammer til indbygget tilstand for Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)