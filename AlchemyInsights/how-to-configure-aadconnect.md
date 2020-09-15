---
title: 646 Sådan konfigurerer du AADConnect
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704483"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunktioner

Azure AD Connect indeholder flere funktioner, der som standard er aktiveret, eller som du kan aktivere senere. Nogle funktioner kræver yderligere konfiguration i bestemte miljøer.

- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrænser, at objekterne synkroniseres til Azure ad. Alle brugere, kontakter, grupper og Windows 10 computer-konti synkroniseres som standard. Du kan medtage eller udelade objekter, der er baseret på domæner, organisationsenheder eller andre attributter.

- [Synkronisering af adgangskode-hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer adgangskode-hashen fra det lokale Active Directory til Azure ad. Dette gør det muligt at administrere adgangskoder på ét sted, men brug af den samme adgangskode i både lokale miljøer og i skyen. Da Active Directory er den autoritative kilde, kan du bruge dine egne adgangskodepolitikker.

- [Nulstilling af adgangskode til selvbetjening (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) gør det muligt for brugerne at nulstille deres egne adgangskoder i skyen, men stadig anvende din lokale adgangskodepolitik.

- [Enheds tilbageførsel](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) gør det muligt for registrerede enheder i Azure ad at blive skrevet tilbage til Active Directory lokalt, så de kan bruges til betinget adgang.

- [Forhindre utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre for mange samtidige objekt sletninger (mere end 500-objekter pr. synkronisering). Du kan ændre denne indstilling, så den opfylder din organisations behov.

- [Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er som standard aktiveret til ekspres installationer og sikrer, at din version af Azure ad Connect altid er aktuel.
