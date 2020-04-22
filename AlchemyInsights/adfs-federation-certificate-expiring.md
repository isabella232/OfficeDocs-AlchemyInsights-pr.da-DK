---
title: Udløb af ADFS-sammenslutningscertifikat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710401"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="75531-102">Udløb af ADFS-sammenslutningscertifikat</span><span class="sxs-lookup"><span data-stu-id="75531-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="75531-103">Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:</span><span class="sxs-lookup"><span data-stu-id="75531-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="75531-104">Installer Microsoft Azure Active Directory Module til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret).</span><span class="sxs-lookup"><span data-stu-id="75531-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="75531-105">Det kan du gøre ved at gå til [Administrer Azure AD ved hjælp af Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="75531-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="75531-106">Følg trinnene i afsnittet "Scenario 1: Ad FS-tokensigneringscertifikatet er udløbet" i afsnittet ["Der opstod et problem med at få adgang til webstedet" fra AD FS, når en bruger i organisationsnetværket logger på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="75531-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="75531-107">Følg trinnene i [Opdater, eller reparer indstillingerne for et domæne i organisationsnetværk i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="75531-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="75531-108">Hvis du vil have mere at vide om fornyelse af sammenslutningscertifikater, skal du se [Forny sammenslutningscertifikater for Microsoft 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="75531-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
