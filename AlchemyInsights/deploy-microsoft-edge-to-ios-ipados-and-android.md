---
title: Installér Microsoft Edge til iOS, iPadOS og Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194483"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="c4b42-102">Installér Microsoft Edge til iOS, iPadOS og Android</span><span class="sxs-lookup"><span data-stu-id="c4b42-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="c4b42-103">Det oversigtsscenarie, der er opsummeret nedenfor, hjælper dig med at tildele Microsoft Edge til brugere af iOS-, iPadOS- og Android-enheder.</span><span class="sxs-lookup"><span data-stu-id="c4b42-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="c4b42-104">Hvis du har blokeret brugere fra at tilmelde sig mobilenheder, fungerer dette guidede scenarie ikke, og brugerne skal selv installere Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="c4b42-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="c4b42-105">Det guidede scenarie omfatter følgende trin:</span><span class="sxs-lookup"><span data-stu-id="c4b42-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="c4b42-106">Forudsætninger</span><span class="sxs-lookup"><span data-stu-id="c4b42-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="c4b42-107">Introduktion</span><span class="sxs-lookup"><span data-stu-id="c4b42-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="c4b42-108">Grundlæggende oplysninger</span><span class="sxs-lookup"><span data-stu-id="c4b42-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="c4b42-109">Konfiguration</span><span class="sxs-lookup"><span data-stu-id="c4b42-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="c4b42-110">Opgaver</span><span class="sxs-lookup"><span data-stu-id="c4b42-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="c4b42-111">Gennemse og oprettelse</span><span class="sxs-lookup"><span data-stu-id="c4b42-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="c4b42-112">Når du har fuldført trinnene i det guidede scenarie, aktiverer Microsoft Intune-politikker følgende funktioner i Microsoft Edge til virksomheder:</span><span class="sxs-lookup"><span data-stu-id="c4b42-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="c4b42-113">Dobbelt identitet</span><span class="sxs-lookup"><span data-stu-id="c4b42-113">Dual identity</span></span>
- <span data-ttu-id="c4b42-114">Integration med Microsoft Intune-appbeskyttelsespolitik</span><span class="sxs-lookup"><span data-stu-id="c4b42-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="c4b42-115">Integration med Azure Active Directory-programproxy</span><span class="sxs-lookup"><span data-stu-id="c4b42-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="c4b42-116">Administrerede favoritter og genveje til startsiden</span><span class="sxs-lookup"><span data-stu-id="c4b42-116">Managed favorites and home page shortcuts</span></span>
