---
title: Arbejde med iOS VPP programmer regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557982"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="a32e9-102">Arbejde med iOS VPP-programmer</span><span class="sxs-lookup"><span data-stu-id="a32e9-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="a32e9-103">Læs, [hvordan du administrerer iOS-apps, der er købt via en diskenhed køb program med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) at vide om funktioner, betingelser og trin til at gøre brug af Apple volumen købe programmet og understøttelse af den i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a32e9-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="a32e9-104">**Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til brugerne, men installationen mislykkedes".</span><span class="sxs-lookup"><span data-stu-id="a32e9-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="a32e9-105">Dette kan ske, hvis der bruges et enkelt VPP-token på tværs af flere udbydere af mobile device management.</span><span class="sxs-lookup"><span data-stu-id="a32e9-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="a32e9-106">VPP tokens fra Apple kan kun bruges sammen med én udbyder.</span><span class="sxs-lookup"><span data-stu-id="a32e9-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="a32e9-107">Hvis du har brugt et VPP-token med flere leverandører, skal du igen overføre token til Intune.</span><span class="sxs-lookup"><span data-stu-id="a32e9-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="a32e9-108">Installationen kan mislykkes også, hvis det samlede antal anlæg overstiger antallet af licenser.</span><span class="sxs-lookup"><span data-stu-id="a32e9-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="a32e9-109">For at få vist en anvendelsesrapport for dine licenser, gå til **Intune Mobile apps** \> siden **App licenser** .</span><span class="sxs-lookup"><span data-stu-id="a32e9-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="a32e9-110">Hvis du vil vide mere om at frigøre licenser i brug, se [i denne artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="a32e9-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
