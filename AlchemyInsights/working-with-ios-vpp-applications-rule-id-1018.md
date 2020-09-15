---
title: Arbejde med iOS VPP-programmer regel-id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688940"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="ddc84-102">Arbejde med iOS VPP-programmer</span><span class="sxs-lookup"><span data-stu-id="ddc84-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="ddc84-103">Læs [, hvordan du administrerer iOS-apps, der er købt via et volumen-købsprogram med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , til at få mere at vide om funktioner, begrænsninger og trin, der skal bruges til at udnytte Apple Volume Purchase og support til det i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="ddc84-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="ddc84-104">**Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til mine brugere, men installationen mislykkedes."</span><span class="sxs-lookup"><span data-stu-id="ddc84-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="ddc84-105">Dette kan ske, hvis der bruges et enkelt VPP-token på tværs af flere udbydere af mobilenheder.</span><span class="sxs-lookup"><span data-stu-id="ddc84-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="ddc84-106">VPP-tokens fra Apple kan kun bruges med én udbyder.</span><span class="sxs-lookup"><span data-stu-id="ddc84-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="ddc84-107">Hvis du har brugt et VPP-token med flere udbydere, skal du overføre tokenet til Intune igen.</span><span class="sxs-lookup"><span data-stu-id="ddc84-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="ddc84-108">Installationen kan også mislykkes, hvis det samlede antal installationer overskrider antallet af licenser.</span><span class="sxs-lookup"><span data-stu-id="ddc84-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="ddc84-109">Hvis du vil have vist en anvendelsesrapport for dine licenser, skal du gå til siden Intune-app-licenser til **Intune** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="ddc84-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="ddc84-110">Du kan få mere at vide om, hvordan du gengiver licenser i brug, i [denne artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="ddc84-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
