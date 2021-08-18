---
title: Aktivér SMTP-godkendelse og -fejlfinding
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321747"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Aktivér SMTP-godkendelse og -fejlfinding

Hvis du vil aktivere SMTP-godkendelse for en postkasse, eller hvis du får fejlen "Klient ikke godkendt", "Godkendelse mislykkedes" eller "SmtpClientAuthentication" med kode 5.7.57 eller 5.7.3 eller 5.7.139, når du forsøger at videresende mails ved at godkende en enhed eller et program med Microsoft 365, skal du udføre disse tre handlinger for at løse problemet:

1. Deaktiver [Azure-sikkerhedsstandardindstillingerne](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ved at slå **Aktivér sikkerhedsstandard til** **Nej.**

    a. Log på Azure-portalen som sikkerhedsadministrator, betinget adgangsadministrator eller global administrator.<BR/>
    b. Gå til Azure Active Directory > **Egenskaber.**<BR/>
    c. Vælg **Administrer sikkerhedsstandardindstillinger.**<BR/>
    d. Angiv **Aktivér sikkerhedsstandard til** **Nej.**<BR/>
    e. Vælg **Gem**.

2. [Aktivér klient-SMTP-indsendelse](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) på den licenserede postkasse.

    a. Fra Microsoft 365 Administration skal du **gå til Aktive** brugere og vælge brugeren.<BR/>
    b. Gå til fanen Mail, og vælg **Administrer mailapps** **under Mailapps**.<BR/>
    d. Kontrollér, **at Godkendt SMTP er** markeret (aktiveret).<BR/>
    e. Vælg **Gem ændringer**.<BR/>

3. [Deaktiver Multi-Factor Authentication (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) på den licenserede postkasse.

    a. Gå til fanen Microsoft 365 Administration, og vælg Aktive brugere i **venstre**  >  **navigationsmenu.**<BR/>
    b. Vælg **Multifaktorgodkendelse.**<BR/>
    c. Vælg brugeren, og **deaktiver Multi-Factor Auth**.<BR/>
