---
title: Fejlfinding af sikkerheds tips til kontrol af registrering af svindel
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658404"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ec418-102">Fejlfinding af sikkerheds tips til kontrol af registrering af svindel</span><span class="sxs-lookup"><span data-stu-id="ec418-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ec418-103">Hvis du får et sikkerheds-tip om, at der står "afsenderen mislykkede vores kontrol af svindel registrering og måske ikke, hvem de ser ud til at være", har afsenderen ikke bestået DKIM-eller SPF-godkendelseskontrol.</span><span class="sxs-lookup"><span data-stu-id="ec418-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ec418-104">Den bedste metode til at løse dette er, at afsenderen godkender sig selv.</span><span class="sxs-lookup"><span data-stu-id="ec418-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ec418-105">Hvis afsenderen sender på dine vegne, skal du godkende dem ved at føje afsenderens IP-adresse til din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="ec418-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ec418-106">Se [fejlfinding af det røde (mistænkelige) sikkerheds tip til registrering af svindel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) numre for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="ec418-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="ec418-107">Her er nogle andre links, der kan hjælpe:</span><span class="sxs-lookup"><span data-stu-id="ec418-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ec418-108">Hvordan Microsoft bruger SPF (afsender politik Framework) til at forhindre forfalskning</span><span class="sxs-lookup"><span data-stu-id="ec418-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="ec418-109">Konfigurere SPF for at forhindre forfalskning</span><span class="sxs-lookup"><span data-stu-id="ec418-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
