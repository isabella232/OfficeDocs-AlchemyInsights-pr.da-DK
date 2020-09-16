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
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664164"
---
# <a name="about-identity-in-yammer"></a>Om identitet i Yammer

Det anbefales, at alle netværk udfører følgende trin for at undgå identitets relaterede problemer:

1. Gennemtving Office 365-identitet efter klargøring af Microsoft 365-konti til brugere i Azure AD for at sikre, at alle brugere logger på med deres primære Microsoft 365-konto. Du kan finde flere oplysninger i [Gennemtving Office 365-identitet for Yammer-brugere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolider flere Yammer-netværk. Ældre Yammer-konfigurationer giver mulighed for at oprette forbindelse til én lejer med flere Yammer-netværk. Hvis du vil have mere at vide, skal du se [Network migration-Konsolider flere Yammer-netværk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Du kan også gennemtvinge licensering til Yammer for at blokere brugere fra Yammer, hvis de ikke har en licens. Du kan finde flere oplysninger i [administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Til sidst skal du overvåge bruger listen for ældre Yammer-netværk og suspendere ældre brugere. Det anbefales, at du suspenderer (deaktiverer) brugere i stedet for at slette dem, da sletningen er uigenkaldelige. Hvis du vil have mere at vide, skal du se [Overvåg Yammer-brugere i netværk, der er forbundet til Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [fjernbrugere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Hvis du konfigurerer Yammer ved hjælp af disse trin, er du også klar til at konfigurere dit Yammer-netværk til Microsoft 365. Hvis du vil have mere at vide, skal du se [konfigurere dit Yammer-netværk til oprindelig tilstand for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).