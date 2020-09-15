---
title: Et af de lokale organisations tjeneste certifikater udløber
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673491"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Et af de lokale organisations tjeneste certifikater udløber

Du kan løse dette problem ved at følge disse trin:
  
- Installer Microsoft Azure Active Directory-modulet til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). Hvis du vil gøre dette, skal du gå til [Azure Active Directory PowerShell til Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg trinnene i afsnittet "scenarie 1: det token-signeringscertifikat for AD FS, der er udløbet" i ["der opstod et problem med at få adgang til webstedet" fra ad FS, når en organisation i organisationsnetværket logger på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Følg trinnene i [, hvordan du opdaterer eller reparerer indstillingerne for et sammenkædet domæne i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Du kan finde flere oplysninger om fornyelse af samlings certifikater under [Certifikatfornyelse for O365 og Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

