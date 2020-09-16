---
title: Send brugerdefinerede meddelelser til Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720640"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="b63db-102">Sådan sender du brugerdefinerede meddelelser til brugerne af administrerede iOS-og Android-enheder</span><span class="sxs-lookup"><span data-stu-id="b63db-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="b63db-103">Brugerdefinerede meddelelser for Intune behandles af appen firma Portal på en brugers enhed.</span><span class="sxs-lookup"><span data-stu-id="b63db-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="b63db-104">Appen opretter derefter push-beskeden på den pågældende enhed.</span><span class="sxs-lookup"><span data-stu-id="b63db-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="b63db-105">Følgende er enheds forudsætninger, der understøtter modtagelse af brugerdefinerede meddelelser, og for appen, så du kan oprette en push-besked:</span><span class="sxs-lookup"><span data-stu-id="b63db-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="b63db-106">Enheden skal have appen firma Portal installeret.</span><span class="sxs-lookup"><span data-stu-id="b63db-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="b63db-107">Enheden skal give appen firma Portal besked om at sende pushmeddelelser.</span><span class="sxs-lookup"><span data-stu-id="b63db-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="b63db-108">Når appen installeres eller opdateres, bliver brugeren bedt om at tillade meddelelser.</span><span class="sxs-lookup"><span data-stu-id="b63db-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="b63db-109">Der skal være installeret Google Play Services på Android-enheder.</span><span class="sxs-lookup"><span data-stu-id="b63db-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="b63db-110">Enheden skal være tilmeldt med Intune.</span><span class="sxs-lookup"><span data-stu-id="b63db-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="b63db-111">Du kan finde flere oplysninger, herunder hvordan du sender en meddelelse, i [dokumentationen til funktionen](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="b63db-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
