---
title: ADFS-sammenslutningscertifikat udløber
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686708"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-sammenslutningscertifikat udløber

Du kan løse dette problem ved at følge disse trin:
  
1. Installer Microsoft Azure Active Directory-modulet til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). For at gøre dette skal du gå til [Administrer Azure AD ved hjælp af Windows PowerShell.](https://aka.ms/aadposh)

2. Følg trinnene i afsnittet "Scenarie 1: AFSNITTET AD FS-tokensigneringscertifikat udløbet" i fejlen "Der opstod et problem med at få adgang til webstedet" fra AD FS, når en bruger i et organisationsnetværk logger på [Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Følg trinnene i [Opdater eller reparer indstillingerne for et organisationsnetværksdomæne i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Du kan få mere at vide om fornyelse af sammenslutningscertifikater under [Forny sammenslutningscertifikater til Microsoft 365 og Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
