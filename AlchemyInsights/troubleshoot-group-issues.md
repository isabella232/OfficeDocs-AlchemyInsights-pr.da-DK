---
title: Fejlfinding af gruppeproblemer
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713438"
---
# <a name="troubleshoot-group-issues"></a>Fejlfinding af gruppeproblemer

**Jeg har brug for at tildele en gruppe til en Azure AD-rolle**

Hvis du vil tildele en Azure Active Directory-gruppe (AD) til en Azure AD-rolle, skal du udføre følgende trin:

1. Opret en ny gruppe – Sådan opretter du en ny gruppe:

    a. Log på Azure AD Administration med rettigheder som rolleadministrator eller global administrator. 
    b. Vælg Azure Active Directory > Grupper > Alle grupper > Ny gruppe. 
    c. Opret gruppen.

2. Tildel rollen til gruppen enten under gruppeoprettelse eller efter, at gruppen er oprettet.

    a. Hvis du vil tildele en rolle til gruppen på tidspunktet for gruppeoprettelsen, skal du slå Til/fra-knappen for Azure AD-roller til og oprette gruppen.
    b. Hvis du vil tildele en rolle til gruppen, efter den er blevet oprettet, skal du gå til fanen Tildelte roller for den nyoprettede gruppe og tildele rollen til gruppen.

**Jeg har brug for at administrere medlemskabet af en gruppe, der er tildelt Rollen Azure AD**

1. For at forhindre udvidelse af rettigheder kan kun den privilegerede rolleadministrator og den globale administrator som standard ændre medlemskabet af en gruppe, der er tildelt en rolle. De kan dog vælge at tildele en ejer til en sådan gruppe og uddelegere denne opgave. Du kan finde flere oplysninger [i Brug skybaserede grupper til at administrere rolletildelinger i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Hvis du vil have mere at vide om almindelige spørgsmål og tip til fejlfinding i forbindelse med tildeling af roller til grupper i Azure AD, skal du se [Fejlfinding af roller, der er tildelt til skygrupper.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dynamiske grupper**

1. Hvis du ikke kan finde de indbyggede brugerattributter, skal du sikre dig, at attributten er på listen over understøttede egenskaber.
2. Hvis du leder efter indbyggede enhedsattributter, skal du sikre dig, at attributten er på listen over enhedsattributter 
3. Ud over de indbyggede bruger- og enhedsattributter kan du også bruge [udvidelsesattributter.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Når du har synkroniseret udvidelsesattributter fra Windows Server AD i det lokale miljø eller fra et tilsluttet SaaS-program, skal attributterne være synlige på rullelisten i regelgeneratoren. Det brugerdefinerede attributnavn kan findes i kataloget ved at forespørge en brugers attribut ved hjælp af PowerShell og søge efter attributnavnet. Disse kan også bruges, når du konstruerer regler i regelsyntaksen.
4. Sørg for, at din lejer har den korrekte licens. Dynamiske grupper kræver, at lejeren har en Azure AD P1 Premium-licens. Du kan få adgang til listen over Azure AD-licensplaner [her.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security-licensplaner kan [tilgås her.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Sørg for, at rollen for den bruger, der opretter den dynamiske gruppe, er en global administrator, intune-administrator, gruppeadministrator eller en brugeradministrator.
6. Giv gruppen tid til at udfylde. Afhængigt af størrelsen på din lejer kan det tage op til 24 timer, før gruppen udfyldes første gang eller efter en regelændring.
7. Du kan finde flere oplysninger [i Oprette attributbaserede regler for dynamisk gruppemedlemskab.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Jeg har brug for at slette en gruppe**

1. Grupper kan slettes fra mappen ved hjælp af Remove-AzureADGroup cmdlet i Azure AD Powershell-modulet.
2. Før du forsøger at slette en synkroniseret gruppe i Azure AD, skal du sikre dig, at du har slettet alle tildelte licenser for at undgå fejl.
3. Du kan finde flere oplysninger om sletning af grupper [under Sletning af en gruppe med en tildelt licens.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Jeg har brug for at gendanne en slettet gruppe**

1. Hvis en Office 365-gruppe slettes, kan den kun gendannes op til 30 dage, før den slettes permanent. Når gruppen er slettet permanent, kan den ikke længere gendannes. Få mere at vide om gendannelse af grupper [her.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Denne funktionalitet understøttes ikke for sikkerhedsgrupper og distributionsgrupper.
3. Sørg for, at du er godkendt til at gendanne en Office 365-gruppe. Globale administratorer, gruppeadministratorer, brugerkontoadministratorer, intune-tjenesteadministratorer, partnerniveau1- eller niveau2-support og ejeren af gruppen kan gendanne en gruppe.
4. Når en dynamisk gruppe slettes og gendannes, ses den som en ny gruppe og udfyldes igen i overensstemmelse med reglen. Denne proces kan tage op til 24 timer.
5. Du kan finde flere oplysninger om gendannelse af en slettet gruppe i Gendan en [slettet Office 365-gruppe i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Politikkonfiguration af gruppeudløb**

1. Denne funktionalitet understøttes kun for Office 365-grupper og ikke for sikkerhedsgrupper og distributionsgrupper understøttes ikke.
2. Konfiguration og brug af udløbspolitikken for Office 365-grupper kræver en Azure AD Premium-licens.
3. I øjeblikket kan der kun konfigureres én udløbspolitik for Office 365-grupper på en lejer.
4. Kun globale administratorer, gruppeadministratorer, brugeradministratorer og ejeren af gruppen kan forny en gruppe.
5. Hvis en Office 365-gruppe er udløbet, slettes den og kan kun gendannes op til 30 dage, før den slettes permanent. Når gruppen er slettet permanent, kan den ikke længere gendannes. Få mere at vide om gendannelse af grupper [her.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Aktivitetsbaseret automatisk fornyelse**

Brugeraktiviteter fra SharePoint, Outlook og Teams kan udløse automatisk fornyelse af grupper. Aktiviteter kontrolleres 35 dage før, en gruppe udløber. Hvis der er aktivitet i den aktuelle gruppelivscyklus, bliver gruppen automatisk fornyet, og mailbeskeder sendes ikke til gruppeejere.

**Beskedtidsindstilling for udløbne grupper**

1. Mailmeddelelser sendes til Office 365-gruppeejere 30 dage, 15 dage og 1 dag før gruppens udløb.
2. Når du første gang konfigurerer udløb, angives grupper, der er ældre end udløbsintervallet, til 35 dage før udløb.
3. Gruppens udløbsdato beregnes på baggrund af gruppens fornyelsesdato og ikke på grundlag af den dato, hvor politikken er opdateret. Hvis udløbspolitikken opdateres, ændres udløbsdatoen ikke.
4. Du kan finde flere oplysninger i [politik for gruppeudløb og](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) fornyelsesmails og gendan en slettet [Office 365-gruppe i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Tilladelse til at oprette en gruppe**

Sørg for, at du er autoriseret til at oprette en ny gruppe. Globale administratorer kan deaktivere oprettelse af grupper i Azure-portalen eller Access-panelet. Du skal muligvis have en administrator for at oprette den nye gruppe for dig eller for at give dig de rette tilladelser.

1. [Opret en ny gruppe, og tilføj medlemmer i Azure-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Opret grupper i Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Deaktiver oprettelse af grupper i Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Administrer, hvem der kan oprette grupper i Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Deaktiver velkomstmeddelelse til Office 365 via Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Administrative Azure AD-roller](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Administrere tilladelser til oprettelse af grupper**

1. Globale administratorer kan administrere tilladelser til oprettelse af grupper af sikkerhed eller Office 365-grupper, der er oprettet i Azure-portalen eller Access-panelet, ved at angive, at brugere kan oprette sikkerhedsgrupper i **Azure-portaler,** eller brugere kan oprette **Office 365-grupper** i indstillinger for Azure-portaler i alle grupper **> Generelt (Indstillinger).**
2. Du kan også begrænse oprettelse af grupper for at vælge en gruppe af brugere, hvis du har en Azure AD P1 Premium-licens.

**Deaktivere velkomstmeddelelse for nye medlemmer af en Office 365-gruppe**

Velkomstmeddelelsen, der sendes til brugere, der er føjet til Office 365-grupper, kan deaktiveres ved at `UnifiedGroupWelcomeMessageEnabled` angive **falsk** i Powershell. Få mere at vide om denne [indstilling her.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













