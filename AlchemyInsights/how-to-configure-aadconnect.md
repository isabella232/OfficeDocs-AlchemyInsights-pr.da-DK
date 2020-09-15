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
# <a name="configure-sync-features"></a><span data-ttu-id="6832b-102">Konfigurere synkroniseringsfunktioner</span><span class="sxs-lookup"><span data-stu-id="6832b-102">Configure sync features</span></span>

<span data-ttu-id="6832b-103">Azure AD Connect indeholder flere funktioner, der som standard er aktiveret, eller som du kan aktivere senere.</span><span class="sxs-lookup"><span data-stu-id="6832b-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="6832b-104">Nogle funktioner kræver yderligere konfiguration i bestemte miljøer.</span><span class="sxs-lookup"><span data-stu-id="6832b-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="6832b-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrænser, at objekterne synkroniseres til Azure ad.</span><span class="sxs-lookup"><span data-stu-id="6832b-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="6832b-106">Alle brugere, kontakter, grupper og Windows 10 computer-konti synkroniseres som standard.</span><span class="sxs-lookup"><span data-stu-id="6832b-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="6832b-107">Du kan medtage eller udelade objekter, der er baseret på domæner, organisationsenheder eller andre attributter.</span><span class="sxs-lookup"><span data-stu-id="6832b-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="6832b-108">[Synkronisering af adgangskode-hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer adgangskode-hashen fra det lokale Active Directory til Azure ad.</span><span class="sxs-lookup"><span data-stu-id="6832b-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="6832b-109">Dette gør det muligt at administrere adgangskoder på ét sted, men brug af den samme adgangskode i både lokale miljøer og i skyen.</span><span class="sxs-lookup"><span data-stu-id="6832b-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="6832b-110">Da Active Directory er den autoritative kilde, kan du bruge dine egne adgangskodepolitikker.</span><span class="sxs-lookup"><span data-stu-id="6832b-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="6832b-111">[Nulstilling af adgangskode til selvbetjening (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) gør det muligt for brugerne at nulstille deres egne adgangskoder i skyen, men stadig anvende din lokale adgangskodepolitik.</span><span class="sxs-lookup"><span data-stu-id="6832b-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="6832b-112">[Enheds tilbageførsel](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) gør det muligt for registrerede enheder i Azure ad at blive skrevet tilbage til Active Directory lokalt, så de kan bruges til betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="6832b-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="6832b-113">[Forhindre utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre for mange samtidige objekt sletninger (mere end 500-objekter pr. synkronisering).</span><span class="sxs-lookup"><span data-stu-id="6832b-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="6832b-114">Du kan ændre denne indstilling, så den opfylder din organisations behov.</span><span class="sxs-lookup"><span data-stu-id="6832b-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="6832b-115">[Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er som standard aktiveret til ekspres installationer og sikrer, at din version af Azure ad Connect altid er aktuel.</span><span class="sxs-lookup"><span data-stu-id="6832b-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
