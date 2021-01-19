---
title: Fejlfinding af brugerproblemer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900876"
---
# <a name="announcements"></a>Meddelelser

Følg Googles vejledning om test kompatibilitet for at teste, om dine apps er berørt. Google-vejledning er tilgængelig i https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Sørg for, at du bruger systemets webvisning eller system browser, når du logger på dine brugere med kunder med kundens Google-konti. Hvis du vil have mere at vide, skal du se [problemer med at logge på programmer ved hjælp af Chrome-browseren](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Jeg kan ikke oprette en ny bruger i min Azure AD-katalog**

Hvis du vil foretage fejlfinding af problemet, der ikke kan oprette en ny bruger i Azure AD, skal du udføre følgende trin:

1. Kontrollér, at du har tilladelse til at oprette en ny standard bruger. Kun den globale administrator-eller Brugeradministratorrolle i Azure Active Directory (AD) kan oprette en ny standard bruger. Hvis du ikke er i en af disse roller, skal du bede en administrator om at føje dig til en af disse roller eller oprette den nye brugerkonto for dig.
2. Kontrollér, at brugernavnet er i et domæne, der er bekræftet i Azure AD. Hvis du ikke har et bekræftet brugerdefineret domænenavn i Azure AD, kan du bruge dit Azure AD-start domæne, som slutter med *. onmicrosoft.com.
3. Sørg for, at brugernavnet er i et domæne, der ikke er sammenkædet til Azure AD, fra din lokale reklame. Brugere kan ikke tilføjes i skyen med domænenavne, der er samlet i det lokale miljø.
4. Sørg for, at ingen andre brugere eller kontaktpersoner allerede har det Brugernavn, du vil tildele den nye bruger. Brugernavne skal være entydige på tværs af Azure AD.
5. Se [Azure ad-roller og administratorer](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for din Azure ad.
6. Se [domænenavnene](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) for din Azure ad.
7. Gennemse [overvågningslogge](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) for at få vist flere detaljerede oplysninger om en nyligt oprettet eller slettet bruger som for hvem, der har udført handlingen og Hvornår.
8. Du kan finde flere oplysninger om at tilføje nye brugere under [brug af Azure-portalen til at oprette en ny bruger i din Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Du kan finde flere oplysninger om tilladelser for administratorroller i Azure AD under [Azure ad administrative roller](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Hvis du vil have mere at vide om at oprette en bruger ved hjælp af Azure AD PowerShell, skal du se [Azure ad PowerShell for at oprette en ny bruger](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problem med selvbetjenings tilmelding**

Hvis du vil foretage fejlfinding af problemer med selvbetjenings tjeneste, skal du udføre følgende trin:

1. Hvis du vil bruge selvbetjenings tjeneste til at logge på med programmer, skal du først aktivere selvbetjenings tjeneste for din lejer. 
2. Hvis du vil aktivere et program til at understøtte selvbetjenings tjeneste, skal du føje det til dit bruger forløb. Næste gang du går til logonsiden for det pågældende program, får du vist en mulighed **_ingen konto? Opret en!_* _. Dette starter selvbetjenings processen for tilmelding.
3. Hvis du vil have mere at vide om, hvordan du bruger selvbetjenings tilmelding til at udfylde en organisation i Azure AD, skal du se selvbetjenings [tjeneste, tilmelding til Azure ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Når du knytter bruger strømmen til et eller flere programmer, kan brugere, der besøger appen, tilmelde sig og få fat i en gæstekonto ved hjælp af de indstillinger, der er konfigureret i bruger strømmen. Hvis du vil have mere at vide om at logge på og få fat i en gæstekonto, kan brugerne se selvbetjenings [tjeneste for gæstebrugere](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problem med at invitere en ekstern bruger**

Hvis du vil foretage fejlfinding af problemer med at invitere en ekstern bruger, skal du udføre følgende trin:

Sørg for, at du sender en brugers invitation til den mailadresse, der svarer til det navn, brugeren logger på med. Hvis du sender invitationen til en brugers proxy-e-mailadresse, kan brugeren ikke indløse den. Du kan finde flere oplysninger i [Azure ad B2B-dokumentationen](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Jeg kan ikke tildele licenser til en bruger**

Hvis du vil foretage fejlfinding af problemer med at tildele licenser til en bruger, skal du udføre følgende trin:

1. Hvis du vil administrere brugerlicenser, skal du sikre dig, at du bruger en konto med en af de nødvendige administratorroller: Global administrator, licens administrator eller Brugeradministrator. Du kan kontrollere brugerens rolle under fanen **katalog rolle** på bruger bladet.
2. Hvis du bruger Azure-portalen, og licens tildelingen mislykkes, skal du klikke på meddelelsen i øverste højre hjørne. Dette åbner et blad med detaljer om, hvad der gik galt. I de fleste tilfælde, der er nok til at forstå og løse problemet.
3. Før du kan tildele en licens til en bruger, skal du kontrollere, at egenskaben **anvendelses placering** er angivet for brugeren. Kontrollér, at brugeren har den pågældende egenskab vist, ved at se fanen **profil** på bruger bladet.
4. Sørg for, at der er nok tilgængelige licenser til det produkt, du forsøger at tildele. Du kan se antallet af licenser, der er tilgængelige i Azure-portalen, ved hjælp af [Azure Active Directory-> licenser-> alle produkter](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Brugeren har muligvis allerede en anden licens, hvis tjenester er i konflikt med dem i den nye licens, du forsøger at tildele. Hvis brugeren for eksempel har tjenesten Exchange Online (plan 1) aktiveret, kan du ikke tildele en licens med Exchange Online (plan 2). Deaktiver en af tjenesterne for at tillade den nye licenstildeling. Hvis du bruger Azure-portalen eller PowerShell-cmdletter, viser siden med **oplysninger om problemet** de specifikke tjenester, der forårsager konflikten.
6. Hvis du forsøger at fjerne en licens, og det er mislykket, kan brugeren have andre licenser med tjenester, der afhænger af de tjenester, du forsøger at fjerne. Hvis du bruger Azure-portalen eller PowerShell-cmdletter, viser fejlmeddelelsen de specifikke tjenester, der har afhængigheder.
7. Hvis du vil have mere at vide om, hvorfor en licens blev tilføjet/fjernet fra en bruger (f. eks. Hvem kan have foretaget ændringer i din organisation), skal du kontrollere overvågningsloggene. Angiv filteret til **licens aktiviteter** for at få vist alle ændringer, herunder den "skuespiller", der har udført dem.
8. Hvis du bruger Exchange Online, er nogle brugere i din lejer muligvis konfigureret forkert med den samme proxyadresse værdi. I sådanne tilfælde kan du se generiske fejlmeddelelser, når en licens handling mislykkes. [Denne artikel](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) indeholder flere oplysninger om dette problem, herunder oplysninger om [, hvordan du opretter forbindelse til Exchange Online ved hjælp af Remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Du kan finde ud af, hvilke brugere i din lejer der indeholder den samme proxyadresse, ved at udføre denne Exchange Online-cmdlet:

Udført

Get-Recipient | hvor {$ _. EmailAddresses-match <user principal name> } | fL Name, RecipientType, emailaddresses





