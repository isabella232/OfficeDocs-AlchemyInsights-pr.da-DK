---
title: Konfigurere domæne tjeneste
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884986"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="3e1fd-102">Det er ikke muligt at aktivere AAD-DS, eller installationen mislykkedes</span><span class="sxs-lookup"><span data-stu-id="3e1fd-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="3e1fd-103">Hvis du vil løse problemet med Azure AD-domæne tjenesten (AAD-DS), der ikke er aktiveret eller ikke kan installeres, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="3e1fd-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="3e1fd-104">Hvis du bruger et allerede eksisterende virtuelt netværk, skal du kontrollere din NSG for regler, der blokerer de porte, der kræves for at synkronisere på en AAD-DOMÆNEadministrator i portalen https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="3e1fd-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="3e1fd-105">Kontrollér, om din fejlmeddelelse er besvaret i denne fejlfindingsvejledning, der er tilgængelig i  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="3e1fd-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="3e1fd-106">Prøv at installere Azure AD-domæne tjenester i et nyt virtuelt netværk.</span><span class="sxs-lookup"><span data-stu-id="3e1fd-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="3e1fd-107">Følg vejledningen i Introduktion til, hvordan du installerer AAD-DS: [oprette og konfigurere Aad-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="3e1fd-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="3e1fd-108">Hvis du har problemer med at installere Azure AD-domæne tjenester, skal du se [fejlfinding i forbindelse med Azure ad-domæne tjenester](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for at løse almindelige fejl, så du kan få tingene til at fungere igen.</span><span class="sxs-lookup"><span data-stu-id="3e1fd-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="3e1fd-109">**AAD-DS kan ikke deaktiveres**</span><span class="sxs-lookup"><span data-stu-id="3e1fd-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="3e1fd-110">AAD-DS kan ikke afbrydes midlertidigt.</span><span class="sxs-lookup"><span data-stu-id="3e1fd-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="3e1fd-111">Hvis du vil stoppe med at bruge dit administrerede domæne, skal det slettes.</span><span class="sxs-lookup"><span data-stu-id="3e1fd-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="3e1fd-112">Hvis du vil slette dit administrerede domæne, skal du se [Slet Aad-domæne tjeneste](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="3e1fd-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



