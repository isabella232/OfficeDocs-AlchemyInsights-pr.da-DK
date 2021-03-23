---
title: Jeg bliver blokeret af Betinget adgang med domæne forbundet enhed
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035721"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Jeg bliver blokeret af Betinget adgang med domæne forbundet enhed

**Stærkt anbefalede værktøjer**

[Fejlfindingsværktøjet til registrering af enheder](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – det værktøj, der hjælper med at foretage fejlfinding af de mest almindelige problemer med enhedsregistrering.

[Test enhedsregistreringsforbindelsesscript](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – det script, der hjælper med at sikre, at en enhed kan få adgang til enhedsregistreringsslutpunkterne under systemkontoen.

[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – det script, der giver dig mulighed for at søge efter og administrere forældede enheder i dit miljø.

Her er nogle almindelige årsager til, at betinget adgang mislykkes på en enhed, der har tilsluttet sig et domæne (Hybrid Azure AD).

1. **Der er ingen Azure AD PRT** på enheden – Du skal sikre dig, at enheden har azure AD Primary Refresh Token (PRT). Du kan finde flere oplysninger om PRT i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Hvis du vil bekræfte, om du har Azure AD PRT, kan du køre kommandoen på enheden og kontrollere, om `dsregcmd/status` "AzureAdPrt" er lig med "JA".

Hvis "AzureAdPrt" er "NEJ", skal du kontrollere følgende:

- Uanset om du har et organisationsnetværk med **AD FS,** og det ikke er tilgængeligt fra dine brugeres hjemmenetværk: I dette tilfælde skal du sikre, at dine "brugernavnmixede" slutpunkter er tilgængelige fra ekstranet. Hvis din AD FS er bag et VPN, skal du sikre dig, at brugerne opretter forbindelse til VPN og logger på enheden igen. Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Om enhedens TPM** er fejlagtig og derfor ikke kan godkende enheden: Kontrollér "tpm.msc" for at se, om tilstanden af TPM er "Klar". Hvis ikke, skal `dsregcmd/leave` du køre og lade enheden slutte sig til Azure AD igen. Prøv derefter igen. Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Du bruger en tredjepartsidentitetsudbyder, som ikke understøtter WS-Trust protokol.** Som beskrevet i vores dokumenter kan hybride Azure AD-enheder ikke fungere i dette tilfælde. Arbejd sammen med din identitetsudbyder for at få support.

2. Brugere bruger **Chrome-browseren uden Windows 10-konti** eller Office-udvidelsen Chrome bruger ikke automatisk PRT på AAD-enheder, der er forbundet med eller **hybrid-AAD-enheder:** Dette fører til fejl i enhedsbaserede betingede adgangspolitikker, hvor fejlmeddelelsen "Ikke-registreret enhed" vises. Hvis du vil bruge Chrome-browseren korrekt, skal du installere "Windows 10-konti" eller "Office-udvidelsen til brugernes Chrome-browser" via SCCM eller Intune. Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Hvis det ikke er muligt at skubbe udvidelsen eksternt, skal du give brugerne besked om, at de manuelt skal installere en af ovennævnte udvidelser for at få adgang til programmer bag enhedsbaseret betinget adgang. Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Enheden var korrekt hybrid i Azure AD, men den blev ved et uheld slettet eller deaktiveret, enten på grund af synkroniseringsændringer i Azure AD Connect eller fra **Azure-portalen:** Hvis dette sker, genkendes enhedsobjektet ikke længere som en fuldt forbundet enhed, selvom statussen "AzureAdJoined" og "PRT" vises som gyldig på enheden.

Du kan løse dette problem ved at `dsregcmd/leave` køre på de berørte enheder og lade dem slutte sig til Azure AD igen. Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Hvis dine enheder bruger Windows 10-opdateringen 1809 med VPN/skyproxy og ser problemer med tilstanden "AzureAdPrt" eller en app med SSO-problemer (outlook opretter ikke forbindelse til postkassen, selvom du havde PRT), skal du sikre dig, at du har denne programrettelse [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) eller den kumulative aprilopdatering [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) for at forhindre PRT-fejl på disse computere.

















