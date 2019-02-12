---
title: ADFS Federation certifikat udløber
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925374"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="68878-102">ADFS Federation certifikat udløber</span><span class="sxs-lookup"><span data-stu-id="68878-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="68878-103">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="68878-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="68878-p101">Installere det Microsoft Azure Active Directory modul til Windows PowerShell på computeren (hvis modulet, der ikke allerede er installeret). For at gøre dette skal du gå til [Administrer Azure AD ved hjælp af Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="68878-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="68878-106">Følg trinnene i det "Scenario 1: AD FS tokensignerende certifikat er udløbet" del af ["Der opstod et problem ved adgang til webstedet" fejl fra AD FS, når et medlem af organisationsnetværk bruger logger på Office 365, Azure, eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="68878-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="68878-107">Følg vejledningen i [at opdatere eller reparere indstillingerne for et domæne i Office 365, Azure, eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="68878-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="68878-108">Hvis du vil vide mere om fornyelse af organisationsnetværk certifikater, se [Forny federation certifikater til Office 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="68878-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

