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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810478"
---
# <a name="issues-with-azure-mfa"></a>Problemer med Azure MFA
Der er et par ting, der skal kontrolleres, hvis brugerne ikke kan logge på med multifaktorgodkendelse (MFA)

1. Den pågældende bruger kan blive blokeret i Azure Active Directory Portal. Hvis det er tilfældet, nægtes godkendelsesforsøg for den pågældende bruger automatisk. [Følg trinnene i denne artikel for at fjerne blokeringen af dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis det ikke virkede at fjerne blokeringen af brugeren, eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, så vil brugeren gå gennem tilmeldingsprocessen igen. [Følg trinnene i denne artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis det er første gang, du har aktiveret MFA, og dine brugere ikke kan logge på klienter, der ikke er i en browser, f.eks. Outlook, Skype osv., er ADAL (Active Directory Authentication Library) ikke aktiveret på dit O365-abonnement. I dette tilfælde skal du oprette forbindelse til Exchange Online Powershell og køre denne cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*