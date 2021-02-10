---
title: Synkronisering af adgangskodehash for domænetjeneste
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177418"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="56368-102">Synkronisering af adgangskodehash for domænetjeneste</span><span class="sxs-lookup"><span data-stu-id="56368-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="56368-103">**Hvis din Azure AD DS-forekomst beder dig om at aktivere synkronisering af adgangskodehash**</span><span class="sxs-lookup"><span data-stu-id="56368-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="56368-104">Du støder på et scenarie, hvor du kører et hybridmiljø med brugere, der synkroniserer fra et lokalt Azure Active Directory-domæneservices (AD DS)-miljø.</span><span class="sxs-lookup"><span data-stu-id="56368-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="56368-105">Dette scenarie opstår, selvom du har synkronisering af adgangskodehash fra den lokale AD DS til din Azure AD-lejer.</span><span class="sxs-lookup"><span data-stu-id="56368-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="56368-106">**Årsag**</span><span class="sxs-lookup"><span data-stu-id="56368-106">**Cause**</span></span>

<span data-ttu-id="56368-107">Dette sker, fordi Azure AD Connect som standard ikke synkroniserer ældre new technology LAN Manager (NTLM) og Kerberos-adgangskodehashes, der er nødvendige for Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="56368-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="56368-108">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="56368-108">**Workaround**</span></span> 

<span data-ttu-id="56368-109">Du skal konfigurere Azure AD Connect for at synkronisere de adgangskodehashes, der kræves til NTLM- og Kerberos-godkendelse.</span><span class="sxs-lookup"><span data-stu-id="56368-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="56368-110">Når Azure AD Connect er konfigureret, synkroniserer en lokal kontooprettelses- eller adgangskodeændringshændelse også de ældre adgangskodehashes til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="56368-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="56368-111">Se her [for at](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) få flere oplysninger om dette og for vejledning til, hvordan du aktiverer synkronisering af adgangskoder i Azure AD DS-hybridmiljøer.</span><span class="sxs-lookup"><span data-stu-id="56368-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>