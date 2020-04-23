---
title: 646 Sådan konfigureres AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722526"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunktioner

Azure AD Connect indeholder flere funktioner, der er aktiveret som standard, eller som du kan aktivere senere. Nogle funktioner kræver yderligere konfiguration i bestemte miljøer.

- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrænser objekterne synkroniseres med Azure AD. Som standard synkroniseres alle brugere, kontakter, grupper og Windows 10-computerkonti. Du kan medtage eller udelade objekter baseret på domæner, OEM'er eller andre attributter.

- [Synkronisering af hash-oplysninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) til adgangskoder synkroniserer hash-værdien af adgangskode fra det lokale Active Directory til Azure AD. Dette giver mulighed for administration af adgangskoder på ét sted, men brugen af den samme adgangskode i både lokale miljøer og cloudmiljøer. Da Active Directory er den autoritative kilde, kan du bruge dine egne adgangskodepolitikker.

- [SSPR (Self-service Password Reset)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) giver brugerne mulighed for at nulstille deres egne adgangskoder i skyen, mens de stadig anvender din lokale adgangskodepolitik.

- [Sikkerhedskopiering af](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) enheder gør det muligt at skrive registrerede enheder i Azure AD tilbage til det lokale Active Directory, så de kan bruges til betinget adgang.

- [Forbyd utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre for mange samtidige objektsletninger (mere end 500 objekter pr. synkronisering). Du kan ændre denne indstilling, så den opfylder organisationens behov.

- [Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er som standard aktiveret for ekspresinstallationer og er med til at sikre, at din version af Azure AD Connect altid er opdateret.
