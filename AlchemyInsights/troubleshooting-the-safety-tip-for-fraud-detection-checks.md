---
title: Fejlfinding af sikkerhedstippet til kontrol af afsløring af svindel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504977"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Fejlfinding af sikkerhedstippet til kontrol af afsløring af svindel

Hvis du får et sikkerhedstip, der siger "Afsenderen har undladt vores kontrol af afsløring af svindel og kan ikke være, hvem de ser ud til at være", har afsenderen ikke bestået enten DKIM- eller SPF-godkendelseskontrol. Den bedste metode til at løse dette er, at afsenderen godkender sig selv. Hvis afsenderen sender på dine vegne, skal du godkende dem ved at føje afsenderens IP-adresse til din SPF-post.
  
Se [Fejlfinding af det røde (mistænkelige) sikkerhedstip til registrering af svindel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for at få flere oplysninger.
  
Her er nogle andre links, der kan hjælpe:
  
- [Sådan bruger Microsoft SPF (Sender Policy Framework) til at forhindre spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurer SPF for at forhindre spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
