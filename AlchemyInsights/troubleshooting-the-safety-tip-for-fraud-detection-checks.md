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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="d413b-102">Fejlfinding i forbindelse med sikkerhed tip til afsløring af svig kontrollerer</span><span class="sxs-lookup"><span data-stu-id="d413b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="d413b-103">Hvis du får en sikkerhed tip, der siger "afsenderen mislykkedes vores kontrol til påvisning af svig og muligvis ikke som de ser ud til at være", og derefter afsenderen kunne bestå enten DKIM eller SPF godkendelseskontrol.</span><span class="sxs-lookup"><span data-stu-id="d413b-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="d413b-104">Den bedste måde at løse dette problem er for afsenderen at godkende sig selv.</span><span class="sxs-lookup"><span data-stu-id="d413b-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="d413b-105">Hvis afsenderen sender på dine vegne, skal du autorisere dem ved at føje afsenderens IP-adresse til din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="d413b-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="d413b-106">Yderligere oplysninger finder du under [fejlfinding rødt (mistænkelige) sikkerhed tip til afsløring af svig kontrollerer](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="d413b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="d413b-107">Her er nogle links, der kan hjælpe:</span><span class="sxs-lookup"><span data-stu-id="d413b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="d413b-108">Hvordan Office 365 bruger afsender policy framework (SPF) for at forhindre spoofing (forfalskning)</span><span class="sxs-lookup"><span data-stu-id="d413b-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="d413b-109">Oprette SPF i Office 365 for at forhindre spoofing (forfalskning)</span><span class="sxs-lookup"><span data-stu-id="d413b-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
