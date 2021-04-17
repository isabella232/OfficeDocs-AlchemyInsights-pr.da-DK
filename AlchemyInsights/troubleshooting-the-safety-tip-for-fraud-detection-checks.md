---
title: Fejlfinding af sikkerhedstip ved registrering af svindelkontroller
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834725"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Fejlfinding af sikkerhedstip ved registrering af svindelkontroller

Hvis du får et sikkerhedstip, hvor der står, at "Afsenderen kunne ikke vores kontroller til registrering af svindel og er muligvis ikke den, de ser ud til at være", så kunne afsenderen ikke bestå enten DKIM- eller SPF-godkendelseskontrollerne. Den bedste metode til at løse dette er, at afsenderen godkender sig selv. Hvis afsenderen sender på dine vegne, skal du godkende vedkommende ved at føje afsenderens IP-adresse til SPF-posten.
  
Se [Fejlfinding af det røde (mistænkelige) sikkerhedstip til registrering af svindel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for at få flere oplysninger.
  
Her er nogle andre links, der kan hjælpe:
  
- [Sådan bruger Microsoft SPF (Sender Policy Framework) til at forhindre spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurer SPF for at forhindre spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
