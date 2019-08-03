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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250159"
---
# <a name="issues-with-mfa"></a>Problemer med MFA
Der er et par ting, hvis brugere ikke logge på ved hjælp af godkendelse i flere niveauer (MFA)

1. Den pågældende bruger være blokeret i Azure Active Directory-Portal. Hvis det er tilfældet, forsøger godkendelse for den pågældende specifikke bruger automatisk nægtes. [Følg trinnene i denne artikel for at fjerne blokeringen af dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis brugeren ikke er blokeret, eller fjerne blokeringen af brugeren ikke kunne hjælpe kan du prøve at nulstille MFA for brugeren, og de vil gå gennem Registrer igen. [Følg trinnene i denne artikel.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis det er første gang, du aktiverede MFA og dine brugere kan ikke logge på andre browsere end klienter som Outlook, Skype osv, er måske ADAL (Active Directory-godkendelse bibliotek) ikke aktiveret på dit abonnement på O365. I dette tilfælde skal du oprette forbindelse til Exchange Online Powershell og køre denne cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*