---
title: Gruppepolitik
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256682"
---
# <a name="group-policy"></a><span data-ttu-id="aae87-102">Gruppepolitik</span><span class="sxs-lookup"><span data-stu-id="aae87-102">Group policy</span></span>

<span data-ttu-id="aae87-103">Indstillinger for bruger- og computerobjekter i Azure Active Directory-domæneservices (Azure AD DS) administreres ofte ved hjælp af Gruppepolitik objekter (GPOs).</span><span class="sxs-lookup"><span data-stu-id="aae87-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="aae87-104">Azure AD DS indeholder indbyggede GPOs til AADDC-brugere og AADDC-computerbeholdere.</span><span class="sxs-lookup"><span data-stu-id="aae87-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="aae87-105">Du kan tilpasse disse indbyggede gruppepolitikobjekter for at konfigurere gruppepolitikken efter behov for dit miljø.</span><span class="sxs-lookup"><span data-stu-id="aae87-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="aae87-106">Medlemmer af gruppen Azure AD DC-administratorer har gruppepolitikadministrationsrettigheder i Azure AD DS-domænet, og de kan også oprette brugerdefinerede GRUPPE'er og organisationsenheder.</span><span class="sxs-lookup"><span data-stu-id="aae87-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="aae87-107">Du kan finde flere oplysninger om, hvad gruppepolitik er, og hvordan den [fungerer, Gruppepolitik oversigt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="aae87-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="aae87-108">I et hybridmiljø synkroniseres gruppepolitikker, der er konfigureret i et lokalt AD DS miljø, ikke med Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="aae87-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="aae87-109">Hvis du vil definere konfigurationsindstillinger for brugere eller computere i Azure AD DS, skal du redigere et af standard-GRUPPEpolitikobjekter eller oprette et brugerdefineret gruppepolitikobjekt.</span><span class="sxs-lookup"><span data-stu-id="aae87-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="aae87-110">I denne artikel [administreres Gruppepolitik,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hvordan du installerer Gruppepolitik-administrationsværktøjerne, hvordan du redigerer de indbyggede gruppepolitikobjekter, og hvordan du opretter brugerdefinerede gruppepolitikobjekter.</span><span class="sxs-lookup"><span data-stu-id="aae87-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



