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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952963"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-sammenslutningscertifikat udløber

Du kan løse dette problem ved at følge disse trin:
  
1. Installér Microsoft Azure Active Directory til Windows PowerShell på computeren (hvis modulet ikke allerede er installeret). For at gøre dette skal du gå [til Administrer Azure AD ved hjælp Windows PowerShell](https://aka.ms/aadposh).

2. Følg trinnene i afsnittet "Scenarie 1: Ad FS-certifikat til signering med token udløbet" i afsnittet "Der opstod et problem med at få adgang til webstedet" fra AD FS, når en bruger i et organisationsnetværk logger på Microsoft 365, Azure eller [Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Følg trinnene i Opdatere [eller reparere indstillingerne for et domæne i organisationsnetværket i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Du kan få mere at vide om at forny sammenslutningscertifikater [under Forny sammenslutningscertifikater for Microsoft 365 og Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
