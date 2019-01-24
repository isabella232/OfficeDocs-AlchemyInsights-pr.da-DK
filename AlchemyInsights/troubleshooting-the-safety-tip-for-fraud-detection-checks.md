---
title: Fejlfinding i forbindelse med sikkerhed tip til afsløring af svig kontrollerer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464099"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Fejlfinding i forbindelse med sikkerhed tip til afsløring af svig kontrollerer

Hvis du får en sikkerhed tip, der siger "afsenderen mislykkedes vores kontrol til påvisning af svig og muligvis ikke som de ser ud til at være", og derefter afsenderen kunne bestå enten DKIM eller SPF godkendelseskontrol. Den bedste måde at løse dette problem er for afsenderen at godkende sig selv. Hvis afsenderen sender på dine vegne, skal du autorisere dem ved at føje afsenderens IP-adresse til din SPF-post.
  
Yderligere oplysninger finder du under [fejlfinding rødt (mistænkelige) sikkerhed tip til afsløring af svig kontrollerer](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Her er nogle links, der kan hjælpe:
  
- [Hvordan Office 365 bruger afsender policy framework (SPF) for at forhindre spoofing (forfalskning)](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [Oprette SPF i Office 365 for at forhindre spoofing (forfalskning)](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

