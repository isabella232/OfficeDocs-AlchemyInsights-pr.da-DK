---
title: Fejlfinding i forbindelse med sikkerhed tip til afsløring af svig kontrollerer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533157"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Fejlfinding i forbindelse med sikkerhed tip til afsløring af svig kontrollerer

Hvis du får en sikkerhed tip, der siger "afsenderen mislykkedes vores kontrol til påvisning af svig og muligvis ikke som de ser ud til at være", og derefter afsenderen kunne bestå enten DKIM eller SPF godkendelseskontrol. Den bedste måde at løse dette problem er for afsenderen at godkende sig selv. Hvis afsenderen sender på dine vegne, skal du autorisere dem ved at føje afsenderens IP-adresse til din SPF-post.
  
Yderligere oplysninger finder du under [fejlfinding rødt (mistænkelige) sikkerhed tip til afsløring af svig kontrollerer](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Her er nogle links, der kan hjælpe:
  
- [Hvordan Office 365 bruger afsender policy framework (SPF) for at forhindre spoofing (forfalskning)](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Oprette SPF i Office 365 for at forhindre spoofing (forfalskning)](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
