---
title: Jeg bliver blokeret af Betinget adgang med kompatibel enhed
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035369"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Jeg bliver blokeret af Betinget adgang med kompatibel enhed

**Stærkt anbefalede værktøjer**

- [Fejlfindingsværktøjet til registrering af enheder](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – et omfattende værktøj, der hjælper med at foretage fejlfinding af de mest almindelige problemer med enhedsregistrering.
- [Test script til registrering af forbindelse til](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) enheder – et værktøj, der bruges til at sikre, at en enhed kan få adgang til enhedsregistreringsslutpunkterne under systemkontoen.
- [Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – et værktøj, der bruges til at søge efter og administrere forældede enheder i dit miljø.

Her er nogle almindelige årsager til, at Betinget adgang mislykkes for  en kompatibel enhed, eller hvorfor dine brugere modtager Du kan ikke komme dertil herfra under en logonanmodning til en organisationsressource.

1. **Enheden er ikke i en påkrævet enhedstilstand med en MDM:**

Valider, at enheden er tilmeldt en godkendt MDM-udbyder som Intune og markeret *som kompatibel.* Du kan finde flere oplysninger om Intune i dette [dokument.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Du kan få en bedre forståelse af enhedsoverholdelse og Intune ved at bruge overholdelsespolitik til at angive regler [for enheder, du administrerer med Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Hvis du har problemer med at tilmelde en enhed med Intune, kan du finde fejlfindingsoplysninger under [Fejlfinding af enhedsregistrering i Microsoft.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Opret en supportanmodning for at få yderligere Support i Intune. Det gør du ved at besøge [siden Hjælp og support i Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Enheden er ikke forbundet til organisationens netværk:**

For at få adgang til organisationsressourcer skal enheden have forbindelse til organisationens netværk, enten via direkte forbindelse eller et virtuelt privat netværk (VPN) og også forbundet til det lokale miljø eller Azure Active Directory. Hvis du vil slutte en arbejdsenhed til organisationens netværk, skal du [se Deltag i din arbejdsenhed i organisationens netværk.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Hvis du vil registrere en personlig/BYOD-enhed, skal [du se Registrer din personlige enhed på organisationens netværk.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Hvis du vil validere, om enheden har tilsluttet sig netværket, kan du følge trinnene for registrerede enheder [her](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) eller arbejdsenheder [her.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) For at begrænse problemet til organisationsnetværksforbindelsen skal du følge retningslinjerne nedenfor:

    1. Log på Windows med din arbejds- eller skolekonto, f.eks alain@contoso.com.
    2. Opret forbindelse til din organisations netværk via et VPN eller DirectAccess.
    3. Når du har forbindelse, skal du trykke på **Windows-tasten+L** for at låse enheden.
    4. Lås din enhed op ved hjælp af din arbejds- eller skolekonto, og prøv derefter at få adgang til den problematiske app eller tjeneste igen.

Hvis du ser **fejlmeddelelsen Du kan ikke komme dertil herfra igen,** er problemet sandsynligvis et andet sted.

3. **Operativsystemet understøttes ikke:**

Sørg for, at du kører en understøttet version af operativsystemet, herunder:

- **Windows-klient:** Windows 7 eller nyere

- **Windows Server:** Windows Server 2008 R2 eller nyere

- **macOS:** macOS X eller nyere

- **Android og iOS:** Nyeste version af android- og iOS-operativsystemer til mobile enheder

4. **Webbrowser understøttes ikke:**

Find understøttede browsere nedenfor. For Chrome-understøttelse med Windows 1703 eller nyere versioner er en Windows 10-kontoudvidelse påkrævet. For Edge 85+ skal brugeren være logget på for at kunne videregive oplysninger om enhedsoverholdelse korrekt. Du kan finde flere oplysninger [her.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 /8.1:** Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune-administreret browser, Safari
- **Android:** **Microsoft Edge:** Intune-administreret browser, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Du kan finde flere oplysninger **om meddelelsen Og** fejlfindingstrinnene [her.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
