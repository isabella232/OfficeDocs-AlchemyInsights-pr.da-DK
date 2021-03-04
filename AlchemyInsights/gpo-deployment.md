---
title: Installation af gruppepolitikobjekt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427086"
---
# <a name="gpo-deployment"></a><span data-ttu-id="58747-102">Installation af gruppepolitikobjekt</span><span class="sxs-lookup"><span data-stu-id="58747-102">GPO Deployment</span></span>

<span data-ttu-id="58747-103">Indstillinger for bruger- og computerobjekter i Azure Active Directory-domæneservices (Azure AD DS) administreres ofte ved hjælp af Gruppepolitik objekter (GPOs).</span><span class="sxs-lookup"><span data-stu-id="58747-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="58747-104">Azure AD DS indeholder indbyggede GPOs til AADDC-brugere og AADDC-computerbeholdere.</span><span class="sxs-lookup"><span data-stu-id="58747-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="58747-105">Du kan tilpasse disse indbyggede gruppepolitikobjekter for at konfigurere gruppepolitikken efter behov for dit miljø.</span><span class="sxs-lookup"><span data-stu-id="58747-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="58747-106">Medlemmer af gruppen Azure AD DC-administratorer har gruppepolitikadministrationsrettigheder i Azure AD DS-domænet, og de kan også oprette brugerdefinerede GRUPPE'er og organisationsenheder.</span><span class="sxs-lookup"><span data-stu-id="58747-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="58747-107">Du kan finde flere oplysninger om, hvad gruppepolitik er, og hvordan den [fungerer, Gruppepolitik Oversigt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="58747-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="58747-108">I et hybridmiljø synkroniseres gruppepolitikker, der er konfigureret i et lokalt AD DS miljø, ikke med Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="58747-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="58747-109">Hvis du vil definere konfigurationsindstillinger for brugere eller computere i Azure AD DS, skal du redigere et af standard-GRUPPEpolitikobjekter eller oprette et brugerdefineret gruppepolitikobjekt.</span><span class="sxs-lookup"><span data-stu-id="58747-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="58747-110">I denne artikel [administreres Gruppepolitik,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hvordan du installerer Gruppepolitik-administrationsværktøjerne, hvordan du redigerer de indbyggede gruppepolitikobjekter, og hvordan du opretter brugerdefinerede gruppepolitikobjekter.</span><span class="sxs-lookup"><span data-stu-id="58747-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
