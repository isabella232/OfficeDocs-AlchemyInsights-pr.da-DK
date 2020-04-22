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
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761377"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Et af dine lokale Federation Service Certifikater udløber

Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:
  
- Installer Microsoft Azure Active Directory Module til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). Det kan du gøre ved at gå til [Azure Active Directory PowerShell til Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg trinnene i afsnittet "Scenario 1: Ad FS-tokensigneringscertifikatet er udløbet" i afsnittet ["Der opstod problemer med at få adgang til webstedet" fra AD FS, når en bruger i organisationsnetværk logger på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Følg trinnene i t[Sådan opdaterer eller reparerer du indstillingerne for et domæne i organisationsnetværk i Office 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Du kan finde flere oplysninger om fornyelse af Federation-certifikater under [Certifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

