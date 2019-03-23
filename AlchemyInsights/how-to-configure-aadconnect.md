---
title: 646 Sådan konfigureres AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779506"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f9f09-102">Konfigurere synkronisering funktioner</span><span class="sxs-lookup"><span data-stu-id="f9f09-102">Configure sync features</span></span>

<span data-ttu-id="f9f09-103">Azure AD Connect indeholder flere funktioner, der aktiveres som standard, eller som du senere kan aktivere.</span><span class="sxs-lookup"><span data-stu-id="f9f09-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="f9f09-104">Nogle funktioner kræver yderligere konfiguration i specifikke miljøer.</span><span class="sxs-lookup"><span data-stu-id="f9f09-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="f9f09-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) grænser objekterne, der synkroniseres Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9f09-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="f9f09-106">Computerkonti synkroniseres som standard, alle brugere, kontaktpersoner, grupper og Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f9f09-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="f9f09-107">Du kan medtage eller udelade objekter baseret på domæner, organisationsenheder eller andre attributter.</span><span class="sxs-lookup"><span data-stu-id="f9f09-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="f9f09-108">[Synkronisering af adgangskode hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer adgangskode hash fra den lokale Active Directory til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9f09-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="f9f09-109">Dette giver mulighed for administration af adgangskoder på ét sted, men anvendelse af den samme adgangskode i både lokale og skybaserede miljøer.</span><span class="sxs-lookup"><span data-stu-id="f9f09-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="f9f09-110">Da Active Directory er den autoritative kilde, kan du bruge din egen adgangskodepolitikker.</span><span class="sxs-lookup"><span data-stu-id="f9f09-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="f9f09-111">[(SSPR) til nulstilling af adgangskode til selvbetjening](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) giver brugerne mulighed at nulstille deres egne adgangskoder i skyen, mens du stadig anvende din lokale adgangskodepolitik.</span><span class="sxs-lookup"><span data-stu-id="f9f09-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="f9f09-112">[Tilbageførsel af enheden](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kan registrerede enheder i Azure Annonce skal skrives tilbage til den lokale Active Directory, så de kan bruges til betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="f9f09-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="f9f09-113">[Undgå utilsigtede sletninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktiveret som standard for at forhindre sletning af for mange samtidige objekt (mere end 500 objekter pr. synkronisering).</span><span class="sxs-lookup"><span data-stu-id="f9f09-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="f9f09-114">Du kan ændre denne indstilling til at opfylde behovene i din organisation.</span><span class="sxs-lookup"><span data-stu-id="f9f09-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="f9f09-115">[Automatisk opgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktiveret som standard for udtrykkelig installationer og hjælper med at sikre, at din version af Azure AD Tilslut altid er aktuelle.</span><span class="sxs-lookup"><span data-stu-id="f9f09-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

