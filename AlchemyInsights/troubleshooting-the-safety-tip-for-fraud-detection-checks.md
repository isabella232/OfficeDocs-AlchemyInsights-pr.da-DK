---
title: Fejlfinding af sikkerhedstip for kontroller til registrering af svindel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955960"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Fejlfinding af sikkerhedstip for kontroller til registrering af svindel

Hvis du får en sikkerhedstip, der siger: "Afsenderen kunne ikke vores kontroller til registrering af svindel, og det er muligvis ikke hvem, de ser ud til at være", så kunne afsenderen ikke bestå enten DKIM- eller SPF-godkendelseskontroller. Den bedste metode til at løse dette er, at afsenderen godkender sig selv. Hvis afsenderen sender på dine vegne, skal du godkende vedkommende ved at føje afsenderens IP-adresse til SPF-posten.
  
Se [Fejlfinding på det røde (mistænkelige) sikkerhedstip kontroller for registrering af svindel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for at få flere oplysninger.
  
Her er nogle andre links, der kan hjælpe:
  
- [Sådan bruger Microsoft SPF (Sender Policy Framework) til at forhindre spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurer SPF for at forhindre spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
