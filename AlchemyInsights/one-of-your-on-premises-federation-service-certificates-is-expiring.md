---
title: Et af dine lokale Federation Service Certifikater udløber
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785297"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="a4774-102">Et af dine lokale Federation Service Certifikater udløber</span><span class="sxs-lookup"><span data-stu-id="a4774-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="a4774-103">Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:</span><span class="sxs-lookup"><span data-stu-id="a4774-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="a4774-104">Installer Microsoft Azure Active Directory Module til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret).</span><span class="sxs-lookup"><span data-stu-id="a4774-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a4774-105">Det kan du gøre ved at gå til [Azure Active Directory PowerShell til Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="a4774-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="a4774-106">Følg trinnene i afsnittet "Scenario 1: Ad FS-tokensigneringscertifikatet er udløbet" i afsnittet ["Der opstod et problem med at få adgang til webstedet" fra AD FS, når en bruger i organisationsnetværket logger på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a4774-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="a4774-107">Følg trinnene i [Sådan opdaterer eller reparerer du indstillingerne for et domæne i organisationsnetværk i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="a4774-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="a4774-108">Du kan finde flere oplysninger om fornyelse af Federation-certifikater under [Certifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a4774-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

