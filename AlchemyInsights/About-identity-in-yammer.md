---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148198"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Det anbefales, at alle netværk udfører følgende trin for at undgå identitetsrelaterede problemer:

1. Gennemtving Office 365-identitet efter klargøring af Microsoft 365-konti til brugere i Azure AD for at sikre, at alle brugere logger på ved hjælp af deres primære Microsoft 365-konto. Du kan finde flere oplysninger under [Gennemtvinge Office 365-identitet for Yammer-brugere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolider flere Yammer-netværk. Ældre Yammer-konfigurationer gør det muligt at oprette forbindelse til flere Yammer-netværk til én lejer. Du kan finde flere oplysninger [under Netværksoverførsel - Konsolidere flere Yammer-netværk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Du kan også gennemtvinge licenser til Yammer for at blokere brugere fra Yammer, hvis de ikke har en licens. Du kan finde flere oplysninger under [Administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Endelig skal du overvåge brugerlisten for ældre Yammer-netværk og suspendere ældre brugere. Det anbefales, at du afbryder (deaktiverer) brugere i stedet for at slette dem, fordi sletningen er irreversibel. Du kan finde flere oplysninger under [Overvåge Yammer-brugere i netværk, der er forbundet med Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [Fjern brugere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Ved at konfigurere Yammer ved hjælp af disse trin er du også klar til at konfigurere Dit Yammer-netværk til Oprindelig tilstand til Microsoft 365. Du kan finde flere oplysninger under [Konfigurere dit Yammer-netværk til Oprindelig tilstand til Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).