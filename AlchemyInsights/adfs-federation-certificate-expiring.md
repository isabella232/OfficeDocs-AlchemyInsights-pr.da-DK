---
title: ADFS-sammenslutningscertifikat udløber
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821945"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-sammenslutningscertifikat udløber

Du kan løse dette problem ved at følge disse trin:
  
1. Installer Microsoft Azure Active Directory-modulet til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). For at gøre dette skal du gå til [Administrer Azure AD ved hjælp af Windows PowerShell.](https://aka.ms/aadposh)

2. Følg trinnene i afsnittet "Scenarie 1: Ad FS-certifikat til signering med token udløbet" i afsnittet "Der opstod et problem med at få adgang til webstedet" fra AD FS, når en bruger i et organisationsnetværk logger på [Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Følg trinnene i Opdatere [eller reparere indstillingerne for et domæne i organisationsnetværket i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Hvis du vil have mere at vide om at forny sammenslutningscertifikater, skal du se [Forny sammenslutningscertifikater til Microsoft 365 og Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
