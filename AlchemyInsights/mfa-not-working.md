---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098596"
---
# <a name="issues-with-azure-mfa"></a>Problemer med Azure MFA
Der er et par ting, der skal kontrolleres, hvis brugerne ikke kan logge på med multifaktorgodkendelse (MFA)

1. Den pågældende bruger kan blive blokeret i Azure Active Directory Portal. Hvis det er tilfældet, nægtes godkendelsesforsøg for den pågældende bruger automatisk. [Følg trinnene i denne artikel for at fjerne blokeringen af dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis det ikke virkede at fjerne blokeringen af brugeren, eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, så vil brugeren gå gennem tilmeldingsprocessen igen. [Følg trinnene i denne artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis det er første gang, du har aktiveret MFA, og dine brugere ikke kan logge på klienter, der ikke bruger browsere, f.eks. Outlook, Skype osv., er ADAL (Active Directory Authentication Library) ikke aktiveret på dit O365-abonnement. I dette tilfælde skal du oprette forbindelse til Exchange Online Powershell og køre denne cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*