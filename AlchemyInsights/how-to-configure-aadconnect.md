---
title: 646 Sådan konfigureres AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541579"
---
# <a name="configure-sync-features"></a>Konfigurere synkronisering funktioner

Azure AD Connect indeholder flere funktioner, der aktiveres som standard, eller som du senere kan aktivere. Nogle funktioner kræver yderligere konfiguration i specifikke miljøer.

- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) grænser objekterne, der synkroniseres Azure AD. Computerkonti synkroniseres som standard, alle brugere, kontaktpersoner, grupper og Windows 10. Du kan medtage eller udelade objekter baseret på domæner, organisationsenheder eller andre attributter.

- [Hash-adgangskodesynkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer adgangskode hash fra den lokale Active Directory til Azure AD. Dette giver mulighed for administration af adgangskoder på ét sted, men anvendelse af den samme adgangskode i både lokale og skybaserede miljøer. Da Active Directory er den autoritative kilde, kan du bruge din egen adgangskodepolitikker.

- [(SSPR) til nulstilling af adgangskode til selvbetjening](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) giver brugerne mulighed at nulstille deres egne adgangskoder i skyen, mens du stadig anvende din lokale adgangskodepolitik.

- [Tilbageførsel af enheden](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kan registrerede enheder i Azure Annonce skal skrives tilbage til den lokale Active Directory, så de kan bruges til betinget adgang.

- [Undgå utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre sletning af for mange samtidige objekt (mere end 500 objekter pr. synkronisering). Du kan ændre denne indstilling til at opfylde behovene i din organisation.

- [Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktiveret som standard for udtrykkelig installationer og hjælper med at sikre, at din version af Azure AD Tilslut altid er aktuelle.
