---
title: Test IRM-konfiguration for nye OME-funktioner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812432"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Test IRM-konfiguration for nye OME-funktioner

For at bekræfte at din Microsoft 365-lejer er konfigureret til at bruge nye OME-funktioner, skal du køre følgende cmdlet'er, mens du har [forbindelse til Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Kontrollér din lejers IRM-konfiguration ved at køre `Get-IRMConfiguration` . Sørg for, at disse værdier er angivet til **Sand:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Kør ved hjælp af dit domæne, afsenderadresse og `Test-IRMConfiguration` modtager. Hvis testen ikke består, skal du undersøge IRM-konfigurationen.

Du kan finde flere oplysninger om, hvordan du bekræfter IRM-konfiguration, [under Bekræfte ny OME-konfiguration Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)