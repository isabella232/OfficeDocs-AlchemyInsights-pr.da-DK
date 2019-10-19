---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545154"
---
# <a name="issues-with-mfa"></a>Problemer med MFA
Der er et par ting at kontrollere, hvis brugerne ikke kan logge ind ved hjælp af multi-faktor-autentificering (MFA)

1. Den berørte bruger kan være blokeret i Azure Active Directory-portalen. Hvis det er tilfældet, vil godkendelsesforsøg for den pågældende bruger automatisk blive nægtet. [Følg trinnene i denne artikel for at fjerne blokeringen af dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis fjerne blokering brugeren ikke hjalp eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, og de vil gå gennem tilmelde processen igen. [Følg trinnene i denne artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis det er første gang, du har aktiveret MFA, og dine brugere ikke kan logge ind på klienter, der ikke er browsere, såsom Outlook, Skype osv., måske er ADAL (Active Directory Authentication Library) ikke aktiveret på dit O365-abonnement. I dette tilfælde skal du oprette forbindelse til Exchange Online PowerShell og køre denne cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*