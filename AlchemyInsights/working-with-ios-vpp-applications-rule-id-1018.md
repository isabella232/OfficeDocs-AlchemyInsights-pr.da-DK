---
title: Arbejde med iOS VPP-programregel-id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719951"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="5e6a6-102">Arbejde med iOS VPP-programmer</span><span class="sxs-lookup"><span data-stu-id="5e6a6-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="5e6a6-103">Læs [Hvordan du administrerer iOS-apps, der er købt via et volumenkøbsprogram med Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) for at få mere at vide om funktioner, begrænsninger og trin til at gøre brug af Apple Volume Purchase Program og support til det i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5e6a6-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="5e6a6-104">**Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til mine brugere, men installationen mislykkedes."</span><span class="sxs-lookup"><span data-stu-id="5e6a6-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="5e6a6-105">Dette kan ske, hvis et enkelt VPP-token bruges på tværs af flere udbydere af administration af mobilenheder.</span><span class="sxs-lookup"><span data-stu-id="5e6a6-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="5e6a6-106">VPP-tokens fra Apple må kun bruges hos én udbyder.</span><span class="sxs-lookup"><span data-stu-id="5e6a6-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="5e6a6-107">Hvis du har brugt et VPP-token med flere udbydere, skal du uploade tokenet til Intune igen.</span><span class="sxs-lookup"><span data-stu-id="5e6a6-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="5e6a6-108">Installationen kan også mislykkes, hvis det samlede antal installationer overstiger antallet af licenser.</span><span class="sxs-lookup"><span data-stu-id="5e6a6-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="5e6a6-109">Hvis du vil se en brugsrapport for dine licenser, skal du gå til siden **Intune Mobile Apps** \> **App-licenser.**</span><span class="sxs-lookup"><span data-stu-id="5e6a6-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="5e6a6-110">Du kan få mere at vide om, hvordan du tilbagegør licenser i brug, i [denne artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="5e6a6-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
