---
title: 646 Sådan konfigureres AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963637"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunktioner

Azure AD Forbind indeholder adskillige funktioner, der er aktiveret som standard, eller som du kan aktivere senere. Nogle funktioner kræver yderligere konfiguration i bestemte miljøer.

- [Filtreringsgrænser](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekterne synkroniseres med Azure AD. Som standard synkroniseres alle brugere, kontakter, grupper Windows 10 computerkonti. Du kan medtage eller udelade objekter baseret på domæner, OUs eller andre attributter.

- [Synkronisering af adgangskodehash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer adgangskodehash fra det lokale Active Directory til Azure AD. Dette tillader adgangskodestyring på ét sted, men brug af den samme adgangskode i både det lokale miljø og skymiljøer. Da Active Directory er den autoritative kilde, kan du bruge dine egne adgangskodepolitikker.

- [SSPR (Self-service password reset)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) giver brugerne mulighed for at nulstille deres egne adgangskoder i skyen, mens du stadig anvender din lokale adgangskodepolitik.

- [Tilbageførsel af](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) enhed gør det muligt at skrive registrerede enheder i Azure AD tilbage til det lokale Active Directory, så de kan bruges til betinget adgang.

- [Undgå utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre for mange samtidige objektsletninger (mere end 500 objekter pr. synkronisering). Du kan ændre denne indstilling, så den opfylder organisationens behov.

- [Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er som standard aktiveret for hurtig installation og er med til at sikre, at din version af Azure AD Forbind altid er opdateret.
