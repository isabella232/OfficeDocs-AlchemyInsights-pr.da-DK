---
title: 451 4.7.0 Midlertidig serverfejl. Prøv igen senere. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812576"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Midlertidig serverfejl. Prøv igen senere. PRX4

Du kan komme ud for et problem, når du sender mail via Smarthost "smtp.office365.com" ved hjælp af SMTP-klientafsendelsesmetoden og modtager fejlen: "451 4.7.0 Midlertidig serverfejl. Prøv igen senere. PRX4 er primært midlertidigt." 

Sørg for, at du ikke bruger en delt postkasse til SMTP-klientindsendelse, da SMTP-klientafsendelsesmetoden kræver en licenseret postkasse for at sende mails. Men hvis du ikke bruger en delt postkasse, og problemet fortsætter, skal du kontrollere følgende:

1. Aktivér klient-SMTP-indsendelse på den licenserede postkasse, der bruges, ved at køre denne PowerShell-kommando:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    ELLER

    1. Gå til Microsoft 365 Administration > **aktive brugere,** og vælg brugeren.
    1. Gå til fanen Mail > **mailapps>** vælg **Administrer mailapps**. 
    1. Kontrollér, at **indstillingen Godkendt SMTP er** markeret (aktiveret).
    1. Vælg **Gem ændringer**.
    
    Kør denne kommando for at aktivere SMTP-godkendelse for en hel organisation:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Bemærk!** Af sikkerhedsmæssige årsager anbefales det, at du kun aktiverer SMTP-godkendelse for den postkasse, der bruges. Indstillingen på brugerniveau tilsidesætter indstillingen på organisationsniveau.

2. Deaktiver Azure-sikkerhedsstandardindstillingerne ved at slå **Aktivér sikkerhedsstandard til** **Nej:**

    1. Log på Azure-portalen som sikkerhedsadministrator, betinget adgangsadministrator eller global administrator.
    1. Gå til Azure Active Directory >**  Egenskaber,** og vælg **Administrer sikkerhedsstandardindstillinger.**
    1. Indstil **til/fra-knappen Aktivér** sikkerhedsstandard til **Nej.**
    1. Vælg **Gem**.

3. Deaktiver Multi Factor Authentication (MFA) på den licenserede postkasse, der bruges.

    1. Gå til Microsoft 365 Administration, og vælg Aktive brugere i **venstre navigationsmenu.**  >  
    1. På siden **Aktive brugere** skal du **vælge Multi-Factor Authentication.**
    1. Vælg brugeren, og deaktiver **Multi-Factor Authentication**.

