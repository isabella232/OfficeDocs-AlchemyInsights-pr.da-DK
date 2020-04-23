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
# <a name="configure-sync-features"></a><span data-ttu-id="cf209-102">Konfigurere synkroniseringsfunktioner</span><span class="sxs-lookup"><span data-stu-id="cf209-102">Configure sync features</span></span>

<span data-ttu-id="cf209-103">Azure AD Connect indeholder flere funktioner, der er aktiveret som standard, eller som du kan aktivere senere.</span><span class="sxs-lookup"><span data-stu-id="cf209-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="cf209-104">Nogle funktioner kræver yderligere konfiguration i bestemte miljøer.</span><span class="sxs-lookup"><span data-stu-id="cf209-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="cf209-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrænser objekterne synkroniseres med Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cf209-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="cf209-106">Som standard synkroniseres alle brugere, kontakter, grupper og Windows 10-computerkonti.</span><span class="sxs-lookup"><span data-stu-id="cf209-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="cf209-107">Du kan medtage eller udelade objekter baseret på domæner, OEM'er eller andre attributter.</span><span class="sxs-lookup"><span data-stu-id="cf209-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="cf209-108">[Synkronisering af hash-oplysninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) til adgangskoder synkroniserer hash-værdien af adgangskode fra det lokale Active Directory til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cf209-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="cf209-109">Dette giver mulighed for administration af adgangskoder på ét sted, men brugen af den samme adgangskode i både lokale miljøer og cloudmiljøer.</span><span class="sxs-lookup"><span data-stu-id="cf209-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="cf209-110">Da Active Directory er den autoritative kilde, kan du bruge dine egne adgangskodepolitikker.</span><span class="sxs-lookup"><span data-stu-id="cf209-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="cf209-111">[SSPR (Self-service Password Reset)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) giver brugerne mulighed for at nulstille deres egne adgangskoder i skyen, mens de stadig anvender din lokale adgangskodepolitik.</span><span class="sxs-lookup"><span data-stu-id="cf209-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="cf209-112">[Sikkerhedskopiering af](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) enheder gør det muligt at skrive registrerede enheder i Azure AD tilbage til det lokale Active Directory, så de kan bruges til betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="cf209-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="cf209-113">[Forbyd utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre for mange samtidige objektsletninger (mere end 500 objekter pr. synkronisering).</span><span class="sxs-lookup"><span data-stu-id="cf209-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="cf209-114">Du kan ændre denne indstilling, så den opfylder organisationens behov.</span><span class="sxs-lookup"><span data-stu-id="cf209-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="cf209-115">[Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er som standard aktiveret for ekspresinstallationer og er med til at sikre, at din version af Azure AD Connect altid er opdateret.</span><span class="sxs-lookup"><span data-stu-id="cf209-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
