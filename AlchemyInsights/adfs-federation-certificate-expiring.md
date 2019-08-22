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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499885"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="3abfd-102">ADFS Federation certifikat udløber</span><span class="sxs-lookup"><span data-stu-id="3abfd-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="3abfd-103">Du kan løse dette problem ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="3abfd-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="3abfd-104">Installere det Microsoft Azure Active Directory modul til Windows PowerShell på computeren (hvis modulet, der ikke allerede er installeret).</span><span class="sxs-lookup"><span data-stu-id="3abfd-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="3abfd-105">For at gøre dette skal du gå til [Administrer Azure AD ved hjælp af Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="3abfd-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="3abfd-106">Følg trinnene i det "Scenario 1: AD FS tokensignerende certifikat er udløbet" del af ["Der opstod et problem ved adgang til webstedet" fejl fra AD FS, når et medlem af organisationsnetværk bruger logger på Office 365, Azure, eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="3abfd-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="3abfd-107">Følg vejledningen i [at opdatere eller reparere indstillingerne for et domæne i Office 365, Azure, eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="3abfd-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="3abfd-108">Hvis du vil vide mere om fornyelse af organisationsnetværk certifikater, se [Forny federation certifikater til Office 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="3abfd-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
