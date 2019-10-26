---
title: ADFS Federation-certifikat udløber
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
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737183"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation-certifikat udløber

Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:
  
1. Installer Microsoft Azure Active Directory-modulet til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). Det kan du gøre ved at gå til [Administrer Azure ad ved hjælp af Windows PowerShell](https://aka.ms/aadposh).

2. Følg trinnene i afsnittet "scenarie 1: AD FS-token-signeringscertifikat udløbet" i ["der opstod et problem med at få adgang til webstedet" fra ad FS, når en federated bruger logger på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Følg trinnene i [opdatere eller reparere indstillingerne for et Fødereret domæne i Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Du kan få mere at vide om fornyelse af organisations certifikater i [forny organisations certifikater til Office 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
