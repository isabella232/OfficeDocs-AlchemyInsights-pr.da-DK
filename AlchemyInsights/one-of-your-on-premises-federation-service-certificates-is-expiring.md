---
title: En af dine lokale Federation Service certifikater udløber
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419686"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>En af dine lokale Federation Service certifikater udløber

Du kan løse dette problem ved at følge disse trin:
  
- Installere det Microsoft Azure Active Directory modul til Windows PowerShell på computeren (hvis modulet, der ikke allerede er installeret). For at gøre dette skal du gå til [Azure Active Directory PowerShell til Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg trinnene i det "Scenario 1: AD FS tokensignerende certifikat er udløbet" del af ["Der opstod et problem ved adgang til webstedet" fejl fra AD FS, når et medlem af organisationsnetværk bruger logger på Office 365, Azure, eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Følg trinnene i t[at opdatere eller reparere indstillingerne for et domæne i Office 365, Azure, eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Du kan finde flere oplysninger om fornyelse af organisationsnetværk certifikater, [Certifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

