---
title: Fejlfinding af sikkerhedstippet i forbindelse med kontrol af afsløring af svindel
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
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759506"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Fejlfinding af sikkerhedstippet i forbindelse med kontrol af afsløring af svindel

Hvis du får et sikkerhedstip, der siger "Afsenderen har ikke udført vores kontrol af afsløring af svindel og muligvis ikke er den, de ser ud til at være", har afsenderen undladt at bestå enten DKIM- eller SPF-godkendelseskontrol. Den bedste metode til at løse dette er, at afsenderen godkender sig selv. Hvis afsenderen sender på dine vegne, skal du godkende vedkommende ved at føje afsenderens IP-adresse til din SPF-post.
  
Se [Fejlfinding af det røde (mistænkelige) sikkerhedstip til kontrol af registrering af svindel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for at få flere oplysninger.
  
Her er nogle andre links, der kan hjælpe:
  
- [Sådan bruger Microsoft SPF (Sender Policy Framework) til at forhindre spoofing](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurer SPF for at forhindre spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
