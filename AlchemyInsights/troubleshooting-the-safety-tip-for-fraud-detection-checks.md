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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="42610-102">Fejlfinding af sikkerhedstippet til kontrol af afsløring af svindel</span><span class="sxs-lookup"><span data-stu-id="42610-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="42610-103">Hvis du får et sikkerhedstip, der siger "Afsenderen har undladt vores kontrol af afsløring af svindel og kan ikke være, hvem de ser ud til at være", har afsenderen ikke bestået enten DKIM- eller SPF-godkendelseskontrol.</span><span class="sxs-lookup"><span data-stu-id="42610-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="42610-104">Den bedste metode til at løse dette er, at afsenderen godkender sig selv.</span><span class="sxs-lookup"><span data-stu-id="42610-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="42610-105">Hvis afsenderen sender på dine vegne, skal du godkende dem ved at føje afsenderens IP-adresse til din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="42610-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="42610-106">Se [Fejlfinding af det røde (mistænkelige) sikkerhedstip til registrering af svindel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="42610-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="42610-107">Her er nogle andre links, der kan hjælpe:</span><span class="sxs-lookup"><span data-stu-id="42610-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="42610-108">Sådan bruger Microsoft SPF (Sender Policy Framework) til at forhindre spoofing</span><span class="sxs-lookup"><span data-stu-id="42610-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="42610-109">Konfigurer SPF for at forhindre spoofing</span><span class="sxs-lookup"><span data-stu-id="42610-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
