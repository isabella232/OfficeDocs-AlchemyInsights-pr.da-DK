---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755125"
---
# <a name="issues-with-azure-mfa"></a>Problemer med Azure MFA
Der er et par ting, du skal kontrollere, hvis brugerne ikke kan logge på ved hjælp af multifaktorgodkendelse (MFA)

1. Den pågældende bruger kan være blokeret i Azure Active Directory-portalen. Hvis det er tilfældet, bliver godkendelsesforsøg for den pågældende bruger automatisk afvist. [Følg trinnene i denne artikel for at fjerne blokeringen af dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis det ikke hjælper at fjerne blokeringen af brugeren, eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, og den gennemgår processen igen. [Følg trinnene i denne artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis dette er første gang, du aktiverer MFA, og dine brugere ikke kan logge på ikke-browser-klienter, såsom Outlook, Skype osv., kan ADAL (Active Directory Authentication Library) ikke være aktiveret på dit O365-abonnement. I dette tilfælde skal du oprette forbindelse til Exchange Online PowerShell og køre denne cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*