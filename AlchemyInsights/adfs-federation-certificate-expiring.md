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
# <a name="adfs-federation-certificate-expiring"></a>Udløb af ADFS-sammenslutningscertifikat

Du kan lÃ ̧se problemet ved at fÃ ̧lge disse trin:
  
1. Installer Microsoft Azure Active Directory Module til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). Det kan du gøre ved at gå til [Administrer Azure AD ved hjælp af Windows PowerShell](https://aka.ms/aadposh).

2. Følg trinnene i afsnittet "Scenario 1: Ad FS-tokensigneringscertifikatet er udløbet" i afsnittet ["Der opstod et problem med at få adgang til webstedet" fra AD FS, når en bruger i organisationsnetværket logger på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Følg trinnene i [Opdater, eller reparer indstillingerne for et domæne i organisationsnetværk i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Hvis du vil have mere at vide om fornyelse af sammenslutningscertifikater, skal du se [Forny sammenslutningscertifikater for Microsoft 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
