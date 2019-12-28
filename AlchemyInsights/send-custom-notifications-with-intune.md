---
title: Send brugerdefinerede meddelelser med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886851"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="62482-102">Sådan sender du brugerdefinerede meddelelser til brugerne af administrerede iOS-og Android-enheder</span><span class="sxs-lookup"><span data-stu-id="62482-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="62482-103">Brugerdefinerede meddelelser for Intune behandles af firmaets Portal-appen på en brugers enhed.</span><span class="sxs-lookup"><span data-stu-id="62482-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="62482-104">Appen opretter derefter push-meddelelsen på den pågældende enhed.</span><span class="sxs-lookup"><span data-stu-id="62482-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="62482-105">Følgende er enheds forudsætninger for at understøtte modtagelse af brugerdefinerede meddelelser, og for at appen kan oprette push-meddelelsen:</span><span class="sxs-lookup"><span data-stu-id="62482-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="62482-106">Enheden skal have appen firma Portal installeret.</span><span class="sxs-lookup"><span data-stu-id="62482-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="62482-107">Enheden skal tillade, at appen firma Portal sender pushmeddelelser.</span><span class="sxs-lookup"><span data-stu-id="62482-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="62482-108">Når appen er installeret eller opdateret, bliver brugeren bedt om at tillade meddelelser.</span><span class="sxs-lookup"><span data-stu-id="62482-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="62482-109">Android-enheder skal have Google Play-tjenester installeret.</span><span class="sxs-lookup"><span data-stu-id="62482-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="62482-110">Enheden skal være tilmeldt Intune.</span><span class="sxs-lookup"><span data-stu-id="62482-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="62482-111">Yderligere oplysninger om, hvordan du sender en meddelelse, finder du i [dokumentationen til funktionen](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="62482-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
